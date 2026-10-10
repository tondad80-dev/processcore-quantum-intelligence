# TDK — Matematické příklady a hranice jejich platnosti

**Autor:** Antonín Dospiva  
**Status:** Veřejná pracovní příloha k [přehledu TDK](README.md). Vlastní explicitní příklady používají známou matematiku a standardní fyzikální pravidla. Nejde o experimentální potvrzení ani o univerzální důkaz pro všechna možná rozšíření TDK.

## 1. Nenulová změna nevylučuje návrat

Vezměme dva stavy A a B s metrikou D(A,B) = 1. Historie A → B → A má nenulovou Diferenci na obou přechodech, ale vrací se do původního stavu.

Podmínka D(S_i+1,S_i) > 0 tedy sama neimplikuje, že všechny stavy v historii jsou navzájem různé. K zákazu návratu by bylo potřeba něco navíc — například přísně monotónní veličinu definovanou na úplném stavu.

Rozšířit stav o stále rostoucí počítadlo historie lze formálně. Takové rozšíření však musí mít nezávislý fyzikální význam; samotné přidání záznamu není důkazem chování vesmíru.

## 2. Počet popisných kroků nevybírá fyzikální trvání

Stejnou fyzikální historii lze podle přípustné reprezentace popsat jedním přechodem nebo dvěma podúseky. Počet kroků je pak 1 nebo 2.

Pokud obě reprezentace znamenají tentýž fyzikální proces, jeho trvání se pouhou změnou popisu nesmí zdvojnásobit. Kandidátní aditivní míra Theta musí pro takové zjemnění splnit:

```text
Theta(e) = Theta(e1) + Theta(e2)
```

Tato konzistence sama nevybírá hodnotu ani unikátní fyzikální míru. Alternativou by byla odvozená kanonická struktura fyzikálních událostí. Z pouhé kladnosti D taková struktura neplyne.

## 3. Přechodová struktura nevybírá pravděpodobnost

Nechť stav A připouští dvě další možnosti B a C. Pro každé p v intervalu (0,1) lze při stejné přechodové kostře zavést:

```text
P(B | A) = p
P(C | A) = 1 - p
```

Všechny tyto modely mají stejné přípustné hrany a normalizované kladné pravděpodobnosti. Přesto dávají odlišné předpovědi.

Důsledek je omezený: model, který specifikuje pouze tuto kostru a kladnost, neurčuje p. Pokud přidáme dynamický zákon nebo symetrii výslovně vyžadující stejné váhy, třída přípustných modelů se změní. Příklad proto není zákazem odvození pravděpodobností z bohatší teorie.

## 4. Stejné primitivní váhy, jiné koherentní složení

Definujme redukovaný podpis S0: bázi (h,v), dvě pojmenované operace U,V, větve UV a VU, jejich pořadové schéma a pouze primitivní přechodové váhy |U_ij|² a |V_ij|². Podpis neobsahuje komplexní fáze ani koherentní složené váhy.

Pro Pauliho matice X,Y a identitu I zvolme:

```text
U = (I - iX) / sqrt(2)
V_delta = [I - i(cos(delta) X + sin(delta) Y)] / sqrt(2)
W_delta = U† V_delta† U V_delta
```

Všechny primitivní váhy jsou pro každé delta rovny 1/2. Přímé násobení však dává:

```text
C_delta = Tr(W_delta)/2 = 1 - sin(delta)^2/2
P_diff = ||(UV_delta - V_delta U) psi||^2/4
       = sin(delta)^2/4
```

Poslední vztah platí pro každý normalizovaný dvousložkový vstup psi v tomto ideálním modelu. W je v SU(2), a proto má reálnou skalární část C; použitý součet výstupů na ní závisí. Fyzikální čtení předpokládá koherentní složení a standardní kvadratické pravidlo detekce.

| delta | Primitivní váhy | P_diff | Složená váha p = |⟨h|UV_delta|h⟩|² |
|---|---:|---:|---:|
| pi/6 | všechny 1/2 | 1/16 | (2 − sqrt(3))/4 |
| pi/2 | všechny 1/2 | 1/4 | 1/2 |

Stejný S0 tedy neurčuje P_diff. Obě operace v každém z uvedených párů nekomutují; ani pouhý příznak nekomutativnosti nepomůže.

**Hranice důkazu:** složená váha p se mění. V této rodině platí P_diff = p(1-p). Pokud podpis obsahuje uvedenou fyzikálně změřenou složenou váhu, oba případy již stejný podpis nemají. Rovněž se liší některé operátorové relace: (UV)³ = −I platí pro delta = pi/2, ale ne pro delta = pi/6.

Proto zde neprokazujeme shodu úplného podpisu TDK, obecného relačního komplexu ani všech fyzikálních invariantů. Výsledek je přesným protipříkladem pouze pro definovaný S0.

Pro tuto kalibrovanou rodinu stačí nezávisle určit r = cos(delta), tedy vzájemný skalární součin rotačních os. Pak P_diff = (1-r²)/4. Tento fyzikální údaj je standardním optickým vstupem, který redukovaný podpis neobsahoval. Jeho zpětné dopočítání z téhož P_diff není nezávislou predikcí.

Motivující externí práce: [Fagundes et al., Sagnac interferometr a geometrická fáze](https://arxiv.org/html/2610.01540v1). Naše parametrická rodina je analytická konstrukce; tabulka nepřebírá experimentální data této práce.

## 5. Samotný fázový faktor nemusí určit výstup

Pro ideální vyvážený dvoucestný stav po eliminaci okolí vezměme:

```text
rho(V,phi) = 1/2 [[1, V exp(-i phi)],
                 [V exp(i phi), 1]],  0 <= V <= 1
```

Vlastní hodnoty jsou (1±V)/2: rho je pozitivní a normalizovaná. Takový stav lze získat z čistého stavu systému a okolí, jehož cestově podmíněné stavy mají reálný překryv V.

Standardní projekce na zápornou vyváženou superpozici dává:

```text
P_minus = (1 - V cos(phi))/2
```

Při phi = 0 mají případy V = 1 a V = 1/2 stejné cestové váhy a fázi, ale P_minus je 0 a 1/4. Chybí velikost koherence.

To neznamená, že úplná teorie s akcí nemůže určit koherenci. Testovaný kandidát dodává pouze fázový faktor; plně specifikovaná teorie může dodat také systém, okolí, přípravu a detekci.

Pro tuto doménu výpočet uzavírají nezávislé mapy na stav rho a měřicí operátory E_y se standardním pravidlem P(y) = Tr(E_y rho). Jejich pouhé převzetí není odvozením vlastní fyziky TDK.

Známý fyzikální kontext: [Preskill, Decoherence, Caltech](https://www.preskill.caltech.edu/ph12b/Ph12b-decoherence-26jan2010.pdf).

## 6. Reprodukovatelná numerická kontrola

Python 3, pouze standardní knihovna. Matice se násobí přímo. Kontrola pokrývá 1001 hodnot delta a 1365 kombinací koherence a fáze; jde o syntetickou kontrolu algebraických vztahů, nikoli měření.

```python
import math
import cmath

def mul(a, b):
    return [[sum(a[i][k]*b[k][j] for k in range(2))
             for j in range(2)] for i in range(2)]

def adj(a):
    return [[a[j][i].conjugate() for j in range(2)]
            for i in range(2)]

def trace(a):
    return a[0][0] + a[1][1]

def residual(a, b):
    return max(abs(a[i][j]-b[i][j])
               for i in range(2) for j in range(2))

I = [[1+0j, 0j], [0j, 1+0j]]
root2 = math.sqrt(2)
U = [[1/root2+0j, -1j/root2], [-1j/root2, 1/root2+0j]]
max_error = 0.0

for j in range(1001):
    d = math.pi*j/1000
    V = [[1/root2+0j, -1j*cmath.exp(-1j*d)/root2],
         [-1j*cmath.exp(1j*d)/root2, 1/root2+0j]]
    for op in (U, V):
        assert residual(mul(adj(op), op), I) < 1e-12
        assert all(abs(abs(z)**2-0.5) < 1e-12
                   for row in op for z in row)
    UV, VU = mul(U, V), mul(V, U)
    W = mul(mul(adj(U), adj(V)), UV)
    C = trace(W)/2
    # Sum squared norm over the first input basis column.
    P = sum(abs(UV[i][0]-VU[i][0])**2 for i in range(2))/4
    p = abs(UV[0][0])**2
    errors = (abs(C-(1-math.sin(d)**2/2)),
              abs(P-math.sin(d)**2/4),
              abs(p-(1-math.cos(d))/2),
              abs(P-p*(1-p)))
    max_error = max(max_error, *errors)
assert max_error < 1e-12

for d in (math.pi/6, math.pi/2):
    V = [[1/root2+0j, -1j*cmath.exp(-1j*d)/root2],
         [-1j*cmath.exp(1j*d)/root2, 1/root2+0j]]
    UV = mul(U, V)
    minusI = [[-1+0j, 0j], [0j, -1+0j]]
    error = residual(mul(mul(UV, UV), UV), minusI)
    print("delta, composite_p, P_diff, cube_relation_residual:",
          d, abs(UV[0][0])**2, math.sin(d)**2/4, error)

coherence_error = 0.0
for j in range(21):
    visibility = j/20
    for k in range(65):
        phi = 2*math.pi*k/64
        rho = [[0.5+0j, visibility*cmath.exp(-1j*phi)/2],
               [visibility*cmath.exp(1j*phi)/2, 0.5+0j]]
        assert abs(trace(rho)-1) < 1e-12
        assert (1-visibility)/2 >= 0
        q = []
        for alpha in (0, math.pi/2, math.pi/4):
            ket = [1/root2+0j, cmath.exp(1j*alpha)/root2]
            E = [[ket[i]*ket[l].conjugate() for l in range(2)]
                 for i in range(2)]
            P = trace(mul(E, rho))
            expected = (1+visibility*math.cos(phi-alpha))/2
            coherence_error = max(coherence_error, abs(P-expected))
            assert -1e-12 <= P.real <= 1+1e-12
            q.append(2*P.real-1)
        coherence_error = max(
            coherence_error, abs(q[2]-(q[0]+q[1])/root2))
assert coherence_error < 1e-12
print("max_matrix_formula_error:", max_error)
print("max_coherence_readout_error:", coherence_error)
print("Numerical checks passed; no empirical claim.")
```

Žádný z příkladů sám nereaktivuje prediktivní větev TDK. Jejich účelem je přesně ukázat, které závěry vyžadují další fyzikální předpoklad a jak kontrolovat rozsah tvrzení.
