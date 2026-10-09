# ASASSN-22av: conditional sensitivity and contamination scenarios for 2070–2097

**Author:** Antonín Dospiva  
**Status:** Public working analysis; AI-assisted preparation and calculation. This note has not undergone independent peer review.

## Conclusion

A reproducible scenario estimate can be made for the proposed observing window. In the independent-error approximation below, the local uncertainty in the PPN parameter gamma is about 0.2845. Replacing the lens-parallax uncertainty by 1% while holding the other errors fixed gives 0.1189; further parallax improvement alone approaches a floor near 0.10.

These are conditional uncertainty estimates around the general-relativity reference gamma = 1. They do not predict the value a future experiment will measure. The floor belongs to this particular error model, rather than to a fundamental limit of the experiment.

A separate, one-point-calibrated contamination model gives illustrative flux thresholds around 2063 and 2066–2067. Those dates are screening results, not demonstrated starting dates for a viable observing campaign.

## Source and scope

The primary source is [Jin et al., *Testing General Relativity with Binary Lens Microlensing Events*, arXiv:2610.11949v1](https://arxiv.org/html/2610.11949v1), especially Tables 1–2 and Sections III–IV. Its ASASSN-22av simulation samples 2070–2097 every three years and yields gamma = 1.017 (+0.244, −0.224). Its approximately 3% outlook concerns combining multiple systems.

We use these inputs:

| Quantity | Value | Symmetric uncertainty used here |
|---|---:|---:|
| Primary-lens Einstein angle, theta_E | 0.724 mas | 0.012 mas |
| Microlensing parallax, pi_E | 0.35 | 0.015 |
| Mass ratio, q | 0.51 | 0.03 |
| Mock angular semimajor axis, a | 2.94 mas | 0.01 mas |
| Mock period, P | 27.976 yr | 0.072 yr |
| Mock lens parallax, pi_L | 0.441 mas | 0.0195 mas |

The asymmetric errors in the source are symmetrized for this calculation. Its flux inputs are K_lens = 18.5 and K_source = 9.27; relative motion is approximately 3 mas/yr, with coupling 1.6e-8 at 144 mas.

This note does not reconstruct the interferometric likelihood, orbital fit, or joint posterior. It is an independent illustrative calculation using published marginal inputs.

## Local uncertainty calculation

Write L for the nominal total lensing mass inferred under GR and D for the dynamical mass. Within the source's assumed weak-field framework,

```text
gamma = 2 L / D - 1
L proportional to theta_E (1 + q) / pi_E
D proportional to (a / pi_L)^3 / P^2
```

For small, independent input errors, define fractional mass uncertainties:

```text
s_L^2 = (sigma_theta / theta_E)^2
      + (sigma_piE / pi_E)^2
      + (sigma_q / (1 + q))^2

s_D^2 = 9 (sigma_a / a)^2
      + 4 (sigma_P / P)^2
      + 9 (sigma_piL / pi_L)^2

sigma_gamma approximately 2 sqrt(s_L^2 + s_D^2), near gamma = 1
```

This gives s_L = 0.05006. The following rows change only the fractional lens-parallax uncertainty:

| Fractional parallax uncertainty | Conditional sigma_gamma | Relative uncertainty at gamma = 1 |
|---|---:|---:|
| 4.42% | 0.2845 | 28.45% |
| 1% | 0.1189 | 11.89% |
| 0.3% | 0.1043 | 10.43% |
| 0.1% | 0.1029 | 10.29% |

The last rows show why reducing the distance error alone eventually has diminishing returns in this proxy. Lensing-mass and orbit errors must also improve.

For illustration, independent uncertainties s_L = 1%, sigma_a/a = 0.1%, sigma_P/P = 0.1%, and sigma_piL/pi_L = 0.3% would yield sigma_gamma = 0.02786. This is a set of conditional requirements for a single-system estimate, not evidence that the measurements are achievable, and not a reproduction of the source's multi-system outlook.

**Covariance is a material limitation.** With mass-estimate correlation rho, the local formula becomes:

```text
sigma_gamma approximately 2 sqrt(s_L^2 + s_D^2 - 2 rho s_L s_D)
```

A derived parallax shares information with the lensing estimate. Treating the marginal quantities independently removes that relationship. The 28.45% proxy therefore cannot be interpreted as a correction to the source's joint-posterior result. Ignoring covariance is not always conservative.

The rows involving improved parallax are hypothetical replacements by independently supplied uncertainties. Additional calibration errors, orbital degeneracies, and systematic biases are absent from this proxy.

## Illustrative contamination screening

Our simplified model assumes constant fluxes and relative proper motion, zero separation at reference year 2022, and circular Gaussian attenuation centered on the lens:

```text
C = 10^[0.4 (K_lens - K_source)] = 4920.395
s(y) = 3 (y - 2022) mas
eta(s) = exp(-k s^2)
k = -ln(1.6e-8) / 144^2 = 0.000865677 mas^-2
r(y) = C eta(s(y))
```

Here r is residual source flux divided by the **total binary-lens flux**. Solving r(y) = r_threshold gives:

| Residual source / total lens flux | Approximate threshold crossing |
|---|---:|
| 100% | 2055 |
| 10% | 2059 |
| 1% | 2063 |
| 0.1% | 2066–2067 |

At 2070 the proxy gives r = 7.87e-5, or about 0.0079%.

Calibration at one point supplies no uncertainty on these dates and does not validate extrapolation. The model omits component orbital displacement, actual centering, wavelength dependence, instrumental leakage, and future instrument changes. A small total-flux fraction is not automatically a similarly small astrometric, phase, or gamma error.

Earlier observations would require a full instrument and orbit simulation showing that residual source light can be fitted without unacceptable bias. Shifting a campaign also changes orbital phase and observing geometry. Consequently, 2063–2067 is a range to investigate under this screening model, not an observing recommendation.

## Reproducible calculation

Run with Python 3; no external packages are needed. The script reproduces both tables and the illustrative single-system precision target.

```python
import math

s_L = math.sqrt(
    (0.012 / 0.724)**2
    + (0.015 / 0.35)**2
    + (0.03 / 1.51)**2
)
s_a = 0.01 / 2.94
s_P = 0.072 / 27.976

print("fractional_parallax_error, sigma_gamma")
for s_pi in (0.0195 / 0.441, 0.01, 0.003, 0.001):
    s_D = math.sqrt((3*s_a)**2 + (2*s_P)**2 + (3*s_pi)**2)
    sigma_gamma = 2 * math.sqrt(s_L**2 + s_D**2)
    print(f"{s_pi:.8f}, {sigma_gamma:.8f}")

contrast = 10**(0.4 * (18.5 - 9.27))
k = -math.log(1.6e-8) / 144**2
print("residual_flux_threshold, year")
for threshold in (1.0, 0.1, 0.01, 0.001):
    year = 2022 + math.sqrt(math.log(contrast / threshold) / k) / 3
    print(f"{threshold:g}, {year:.4f}")

r_2070 = contrast * math.exp(-k * (3 * (2070 - 2022))**2)
target = 2 * math.sqrt(0.01**2 + (3*0.001)**2
                       + (2*0.001)**2 + (3*0.003)**2)
print(f"residual_fraction_2070 = {r_2070:.10g}")
print(f"illustrative_sigma_gamma_target = {target:.8f}")
```

## Interpretation boundary

This note supports a transparent assessment of conditional test sensitivity. It supplies no physical prediction from TDK and no evidence of a departure from general relativity. Gamma = 1 is the reference assumption.

This research note is separate from claims about ProcessCore software. AI assistance was used in drafting and calculation; the numerical steps are exposed above so readers can check them independently.
