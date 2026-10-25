# Radio Frequency Technology (`HF3`) – Lernstrategie & Übersicht

- **Haupt-Lernstrategie (alle 4 Fächer):** [`../Readme.md`](../Readme.md)
- **Ausführliche Formelsammlung (PDF, 42 Seiten):** [`Formelsammlung_HF3.pdf`](./Formelsammlung_HF3.pdf) (auch im Hauptverzeichnis [`../Formelsammlung_HF3.pdf`](../Formelsammlung_HF3.pdf))
- **Realistische Probeklausur inkl. Musterlösung (PDF):** [`Probeklausur_HF3.pdf`](./Probeklausur_HF3.pdf) (auch im Hauptverzeichnis [`../Probeklausur_HF3.pdf`](../Probeklausur_HF3.pdf))
- **Vorlesungsskript:** [`Vorlesung/RFT (HF3).pdf`](./Vorlesung/RFT%20(HF3).pdf) & [`Vorlesung/HF_1_altes_damaligen_material.pdf`](./Vorlesung/HF_1_altes_damaligen_material.pdf)
- **12 Übungsblätter:** [`Übungen/Exercise questions winter term 2020-2021/`](./Übungen/Exercise%20questions%20winter%20term%202020-2021/)

---

## 1. Prüfungsformat & Konkreter Lernfahrplan
- **Dauer & Hilfsmittel:** 120 Minuten, **Open Book** (alle gedruckten und handschriftlichen Unterlagen erlaubt, keine programmierbaren/kommunikationsfähigen Geräte).
- **Aufgabenstruktur:** Kombination aus Rechenaufgaben eng entlang der 12 Übungsblätter und konzeptionellen **„Short Questions“** (wie am Ende der Übungsblätter 5–12: Feldlinienbilder, Sonden-/Schlitzplatzierung, Frequenzverschiebungen ohne Rechnung begründen).
- **5-Blöcke-Fahrplan durch die Übungen:**
  1. **Übung 1–3:** S-Parameter, Unitarität ($[S]^H[S]=[E]$), verlustbehaftete Leitungen ($\cosh/\sinh$), Smith-Chart-Stub-Matching, Microstrip (Wheeler) & Stripline-Teiler.
  2. **Übung 4–6:** Rechteckhohlleiter ($\text{TE}_{mn}, \text{TM}_{mn}$, Cutoff-Attenuator, Leistungsfluss $P = \frac{ab}{4Z_{\text{TE}}}E_{\max}^2$, Wanddämpfung $\alpha_c$, Stift-/Schleifen-/Schlitzkopplung).
  3. **Übung 7–8:** Koaxialkabel, Rundhohlleiter ($\text{TE}_{11}, \text{TM}_{01}, \text{TE}_{01}/\text{TM}_{11}$-Entartung, Mehrwege-Dispersion) & Dielektrische Filmwellenleiter (Slab Waveguides, $\text{TM}_0$ ohne Cutoff).
  4. **Übung 9–10:** Verkürzter $\lambda/4$-Koaxialresonator mit Endkapazität, Rechteck- und Zylinder-Hohlraumresonatoren ($\text{TE}_{101}, \text{TM}_{010}, \text{TE}_{011}$), Gütefaktoren ($Q_0, Q_L, Q_{\text{ext}}$, $|S_{21}(f_r)| = 1 - Q_L/Q_0$) und Leitfähigkeits-Skalierung ($Q_c \propto \sqrt{\sigma}$).
  5. **Übung 11–12:** Ferrite ($2{,}8\,\text{MHz/Oe}$, $\mu_\pm$, Faraday-Drehung, Isolator/Zirkulator), Oszillator-Phasenrauschen (Leeson-Formel), Y-Faktor-Rauschmessung und VNA-Kalibrationsrestfehler.

## 2. Wichtigste Stolpersteine
- **$\text{Np/m}$ vs. $\text{dB/m}$:** Alle physikalischen Formeln für $\alpha_c, \alpha_d$, $\tanh(\gamma l)$ und $Q_0 = \frac{\beta}{2\alpha}$ verlangen **$\text{Np/m}$** ($\alpha_{[\text{Np/m}]} = \alpha_{[\text{dB/m}]} / 8{,}6859$)!
- **Spitzenwerte im Poynting-Vektor:** In $P_{\text{TE}_{10}} = \frac{ab}{4Z_{\text{TE}}}E_{\max}^2$ ist $E_{\max}$ der Spitzenwert (Faktor $1/2$ aus Zeitmittelung).
- **Moden-Entartung & Symmetrie im Rundhohlleiter:** $\text{TE}_{01}$ und $\text{TM}_{11}$ teilen sich $p'_{01} = p_{11} = 3{,}8317$; ein koaxialer Übergang regt aus Symmetriegründen ($m=0$) nach $\text{TM}_{01}$ erst **$\text{TM}_{02}$** ($p_{02} = 5{,}520$) an!

