# Introduction to CMOS Analog IC Design (`Intro_to_CMOS`) – Lernstrategie & Übersicht

- **Haupt-Lernstrategie (alle 4 Fächer):** [`../Readme.md`](../Readme.md)
- **Ausführliche Formelsammlung (PDF, 45 Seiten):** [`Formelsammlung_Intro_to_CMOS.pdf`](./Formelsammlung_Intro_to_CMOS.pdf) (auch im Hauptverzeichnis [`../Formelsammlung_Intro_to_CMOS.pdf`](../Formelsammlung_Intro_to_CMOS.pdf))
- **Realistische Probeklausur inkl. Musterlösung (PDF):** [`Probeklausur_Intro_to_CMOS.pdf`](./Probeklausur_Intro_to_CMOS.pdf) (auch im Hauptverzeichnis [`../Probeklausur_Intro_to_CMOS.pdf`](../Probeklausur_Intro_to_CMOS.pdf))
- **Vorlesungsfolien (`Introduction` + `Chapter 01`–`06`):** [`Vorlesung/Presentation Files/`](./Vorlesung/Presentation%20Files/)
- **Übungsblätter (`Ex1`–`Ex7`):** [`Übungen/lntroduction to CMOS Analog lntegrated Circuit Design - Exercise/`](./Übungen/lntroduction%20to%20CMOS%20Analog%20lntegrated%20Circuit%20Design%20-%20Exercise/)

---

## 1. Prüfungsformat & Konkreter Lernfahrplan
- **Dreistufiges Standard-Rechenschema für jede Aufgabe:**
  1. **DC-Arbeitspunkt & Dimensionierung:** Aus $I_D$ und $V_{GSeff} = V_{GS} - V_{th}$ das Verhältnis $(W/L) = \frac{2 I_D}{\mu C'_{ox} V_{GSeff}^2 (1 + \lambda V_{DS})}$ berechnen und Sättigung ($V_{DS} \ge V_{GSeff}$) prüfen.
  2. **Kleinsignalparameter am Arbeitspunkt:** $g_m = \frac{2 I_D}{V_{GSeff}} = \sqrt{2\mu C'_{ox}\frac{W}{L}I_D}$, $g_{ds} = \frac{1}{r_{ds}} = \lambda I_D$, $g_{mb} = \eta g_m$.
  3. **Kleinsignal-Übertragung & Frequenzgang:** $G_m = Y_{21}$, $r_{out} = 1/Y_{22}$, $A_v = -G_m r_{out}$ sowie Knotenkapazitäten (inkl. Miller-Kapazität $C_M = (1 + |A_v|)C_{GD}$), Pole $\omega_{p,i} = -\frac{1}{R_i C_i}$ und RHP-Nullstellen $\omega_z = +\frac{g_m}{C_{GD}}$.
- **Schwerpunkte der 7 Übungen (`Ex1`–`Ex7`):**
  - `Ex1` & `Ex2`: Parameterextraktion ($\lambda, V_{th}$) aus Kennlinienpunkten, MOSFET-Kapazitäten in Cutoff/Linear/Sättigung, Push-Pull-Inverter-Verstärker.
  - `Ex3`: Mehrstufige Stromspiegel-Ketten mit Kanallängenmodulation $\lambda$, $V_{\text{OUT,opt}} = V_{GS1,2}$ und $R_{L,\text{max}}$.
  - `Ex4`, `Ex4-2`, `Ex4-3`: CS-Rückwärtsentwurf aus Gain & Swing, Regulated Cascode ($r_{out} \approx A g_{m4} r_{ds4} r_{ds3}$), Source-Folger mit Body-Effekt.
  - `Ex5`: Bode-Diagramm, Phasenreserve $\text{PM}$, CS-Frequenzgang über Y-Parameter.
  - `Ex6` & `Ex7`: Differenzstufe ($\text{ICMR}$ mit/ohne Body-Effekt, $\text{CMRR} \approx 2g_m r_{ss}$), 5-Transistor-OTA (Mirror-Pol) und mehrstufiger Current-Mirror-OTA (Signalpfade, 4 Pole, 5 Nullstellen).

## 2. Wichtigste Stolpersteine
- **Zwei Body-Effekt-Formeln:** Ist $2\Phi_F$ gegeben (`Ex4`), nutze $V_{th} = V_{th0} + \gamma(\sqrt{2\Phi_F + V_{SB}} - \sqrt{2\Phi_F})$; ist kein $2\Phi_F$ gegeben (`Ex6`), nutze $V_{th} = V_{th0} + \gamma\sqrt{V_{SB}}$!
- **Differenzstufe:** Im Ruhepunkt fließt durch jeden Zweig nur **$I_{D1,2} = I_{SS}/2$**!
- **Miller-Effekt bei Kaskoden (`Chapter 05`):** Die einseitige Kaskode minimiert den Miller-Effekt ($r_{in,S2} \approx 2/g_{m2}$), während bei der Vollkaskode die hochohmige Kaskodenlast den Eingangswiderstand von $M_2$ auf $r_{ds1} \parallel r_{ds4}$ anhebt!

