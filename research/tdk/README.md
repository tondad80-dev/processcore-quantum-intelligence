# TDK — Teorie dimenzionální kaskády

### Vesmír jako proces: změna, vztahy a hranice fyzikálního popisu

**Autor:** Antonín Dospiva  
**Veřejný přehled:** 10. října 2026  
**Status:** Nezávislý výzkumný projekt. Aktivní koncepční rámec; vlastní prediktivní fyzikální teorie dosud není uzavřena ani empiricky potvrzena.

> TDK zkoumá, co lze o fyzikálním systému odvodit z jeho změn, vztahů a procesní historie — a jaký další fyzikální obsah je potřeba, aby z takového popisu vznikla měřitelná předpověď.

## 1. Základní otázka

Lze vesmír popsat jako jeden provázaný proces, v němž známé objekty představují relativně stabilní struktury a lokální mechanismy?

TDK tuto možnost používá jako výzkumnou perspektivu. U konkrétního systému sleduje, které změny proběhly, jak spolu souvisejí, co je generuje a co se stane při dosažení hranice určitého režimu. Jednota procesu sama však neurčuje jeho zákony, determinismus ani jedinečný další stav.

Výraz „dimenzionální kaskáda“ pochází z původní hypotézy vrstev a projekcí mezi nimi. Postupné kritické prověřování přesunulo těžiště projektu k přesněji vymezenému procesnímu rámci. Původní název označuje výzkumnou kontinuitu; nepředstavuje důkaz dalších rozměrů.

## 2. Jádro současného rámce

| Rozlišení | Obsah | Co musí dodat fyzika |
|---|---|---|
| Stav a změna | Přechod musí odpovídat relevantní změně systému. | Které stavy a rozdíly jsou fyzikálně významné. |
| Pořadí a trvání | Pořadí událostí se liší od jejich doby trvání. | Hodinové a časové vztahy. |
| Lokální dokončení a další vývoj | Konec jednoho mechanismu může znamenat přechod do jiného režimu. | Podmínky přechodu a nový dynamický zákon. |
| Pozorovaný stav a historie | Stejný pozorovaný koncový stav nemusí stačit pro stejnou budoucí předpověď. | Relevantní paměť, skryté proměnné nebo úplnější stav. |
| Fyzická odlišnost a měřitelnost | Rozdíl uvnitř modelu nemusí být dostupný danému měření. | Vazbu modelu na experimentální výsledky. |

Pro jednu reprezentovanou historii lze psát:

```text
S0 -> S1 -> ... -> Sn
tau = pořadí nebo procesní hloubka v daném popisu
T = součet fyzikálních dob mezi příslušnými událostmi
D(Si+1, Si) > 0 pro přechody, které počítáme jako skutečnou změnu
```

Diference D, procesní trvání a přenos fáze jsou různé matematické objekty. Nelze je automaticky zaměnit.

Rozdělení jedné události na více popisných kroků navíc mění jejich počet. Samotné počítadlo proto není odvozeným fyzikálním časem. Relační program času potřebuje fyzikálně určené události nebo míru procesu, která přežije přípustné zjemnění popisu, a vazbu na skutečné hodiny.

## 3. Dvě větve projektu

**TDK-C — koncepční a formální rámec.** Organizuje stavy, vztahy, historii a změny režimů. Zkoumá, které závěry z této struktury plynou a které vyžadují další předpoklady. Tato větev zůstává aktivní.

**TDK-P — prediktivní fyzikální větev.** Má dodat konkrétní fyzikální zákon a dostupnou předpověď. Její rozvoj je pozastaven do nalezení nezávislého fyzikálního principu nebo odpovídajícího nového vstupu. Žádný dosavadní kandidát nesplnil požadavky na její reaktivaci.

TDK je samostatný projekt. Technické umístění těchto dokumentů ve společném repozitáři nevytváří vztah vědeckého potvrzení s ProcessCore.

## 4. Co dosavadní práce skutečně přinesla

Hlavním výsledkem je zpřesnění nutných struktur a odstranění neoprávněných zkratek. Některé výsledky jsou aplikacemi známé matematiky; nejsou vydávány za nové fyzikální zákony.

**Procesní kostra neurčuje dynamiku.** Stejný prostor možností může nést různé přechodové pravděpodobnosti. Pořadí, konzistence nebo symetrie samy nevybírají všechny jejich fyzikální hodnoty.

**Historie může být pro předpověď podstatná.** Nestačí vždy uchovat právě pozorovaný endpoint. Potřebná je ta informace o minulosti, která mění předpovědi přípustných pokračování. Z toho však neplyne povinnost uchovávat celou minulost ani zákaz všech opakování.

**Změna každého sousedního stavu nevylučuje návrat později.** Podmínka D > 0 pro každý krok připouští například A → B → A. „Spirála“ je názornou pracovní interpretací vývoje; obecný zákaz přesné rekurence celého vesmíru tím není prokázán.

**Pořadí neuzavírá geometrii.** Rekonstrukce geometrie potřebuje další fyzikální obsah: například míru objemu či měřítka, pravidla šíření signálů, volného pohybu a porovnání hodin. TDK tyto struktury zatím společně neodvodila.

**Primitivní pozitivní váhy mohou ztratit interferenční informaci.** V konkrétní polarizační rodině lze zachovat váhy jednotlivých operací a měnit výstup jejich koherentní kompozice. Audit současně ukázal, že složené váhy a některé operátorové relace se mění. Tento pár proto nedokazuje shodu celého fyzikálního podpisu TDK ani univerzální no-go pro relativní fázi.

**Samotná fáze není vždy úplným fyzikálním vstupem.** V omezeném dvoucestném modelu může stejná relativní fáze při jiné koherenci dát jiný interferenční výstup. Predikce vyžaduje specifikovat stav, přípravu a měření. Vztah exp(iS/hbar) bez určení akce a relevantních fyzikálních podmínek tento problém sám neřeší.

Konkrétní příklady, jejich předpoklady a spustitelnou kontrolu obsahuje [matematická příloha](mathematical-examples.md).

## 5. Nejnovější veřejná analýza: mikročočkování

[Scénářový výpočet pro ASASSN-22av a období 2070–2097](asassn22av-conditional-forecast.md) posuzuje citlivost budoucího testu a kontaminaci světlem zdroje.

V nezávislé lokální aproximaci dává základní sada vstupů nejistotu gamma přibližně 0,2845. Hypotetická paralaxa s chybou 1 % při ostatních pevných chybách snižuje odhad na 0,1189; další zpřesnění samotné paralaxy se blíží hranici kolem 0,10 v této proxy.

Odhad nedodává budoucí centrální hodnotu gamma ani TDK předpověď. Nezahrnuje úplnou kovarianci původní studie. Orientační roky 2063–2067 vycházejí z jednoduchého modelu světelné kontaminace; nejsou prokázaným termínem proveditelného měření.

Jde o ukázku, jak projekt může vymezovat testovací kapacitu bez tvrzení o objevu nové fyziky.

## 6. Původní motivy a jejich dnešní status

| Motiv | Současná hranice tvrzení |
|---|---|
| Vrstvy a dimenzionální projekce | Historická a otevřená interpretační hypotéza; mechanismus není odvozen. |
| Hvězda jako zdroj, černá díra jako opačný tok | Není univerzálním zákonem současného jádra. |
| Vznik nového vodíku dimenzionálním tokem ve hvězdách | Vyřazeno z jádra. |
| Temná hmota jako gravitační stín | Není odvozeným vysvětlením ani potvrzeným výsledkem. |
| Univerzální minimální diference | Není potvrzenou konstantou aktivní fyzikální baseline. |
| Skrytá procesní vrstva | Logická možnost; bez konkrétní měřicí vazby není identifikovanou novou fyzikou. |
| Astronomické anomálie či známé kvantové efekty | Možné podněty pro výzkum; samy nepotvrzují TDK. |

## 7. Rozhodující další cíl

Chybí nezávislé fyzikální pravidlo, které z procesního popisu určí nebo omezí skutečný stav, dynamiku či měřicí statistiku.

Úspěšný kandidát musí mít výslovnou doménu, jednotky a společnou omezenou sadu parametrů. Musí respektovat příslušné známé fyzikální testy a dát alespoň jednu dostupnou předpověď, která jej v předem vymezených podmínkách rozliší od zvoleného standardního modelu.

Predikce a rozhodovací pravidlo musí vzniknout před potvrzovacími daty. Data použitá k návrhu hypotézy slouží k jejímu vzniku; nezávislé potvrzení vyžaduje oddělený test.

Pouhé přejmenování známého mechanismu, přidání volné funkce nebo přizpůsobení již viděné anomálii tento cíl nesplňuje.

## 8. Veřejné materiály a metodika

- [Matematické příklady a reprodukovatelná kontrola](mathematical-examples.md).
- [ASASSN-22av: podmíněný odhad pro 2070–2097](asassn22av-conditional-forecast.md).
- [Surya: The causal set approach to quantum gravity](https://arxiv.org/abs/1903.11544) — související známý výzkumný směr; není důkazem TDK.
- [Fagundes et al.: Measuring Geometric Phase based on Indefinite Causal Order in a Sagnac Interferometer](https://arxiv.org/html/2610.01540v1) — externí optická práce motivující omezený analytický příklad.

Přehled vychází z prověřeného projektového jádra, evidence jeho limitů a navazujících pracovních analýz fáze, koherence a mikročočkování. Při přípravě textu a kontrole výpočtů byla použita generativní AI. Veřejné texty dosud neprošly nezávislým odborným recenzním řízením. Numerická kontrola ověřuje výpočet, nikoli fyzikální pravdivost hypotézy.

### English abstract

TDK (Theory of Dimensional Cascade) is an independent research project studying physical systems through change, relations, process history, and transitions between dynamical regimes. Its active conceptual branch separates process order from duration, endpoint descriptions from predictive state, and mathematical distinction from operational distinguishability. Current work identifies missing physical inputs rather than establishing new physics. A predictive branch remains suspended pending an independently motivated law with an accessible, prespecified discriminator against established models. The public materials include scoped mathematical counterexamples and a conditional ASASSN-22av sensitivity calculation; neither constitutes empirical confirmation of TDK.
