# Microwave Engineering (`MWE`) – Lernstrategie & Übersicht

- **Haupt-Lernstrategie (alle 4 Fächer):** [`../Readme.md`](../Readme.md)
- **Ausführliche Formelsammlung (PDF, 38 Seiten):** [`Formelsammlung_Microwave_Engineering.pdf`](./Formelsammlung_Microwave_Engineering.pdf) (auch im Hauptverzeichnis [`../Formelsammlung_Microwave_Engineering.pdf`](../Formelsammlung_Microwave_Engineering.pdf))
- **Realistische Probeklausur inkl. Musterlösung (PDF):** [`Probeklausur_Microwave_Engineering.pdf`](./Probeklausur_Microwave_Engineering.pdf) (auch im Hauptverzeichnis [`../Probeklausur_Microwave_Engineering.pdf`](../Probeklausur_Microwave_Engineering.pdf))
- **Original-Altklausur WiSe 22/23:** [`old exams/MWE_WS2223_v1_eng_sol.pdf`](./old%20exams/MWE_WS2223_v1_eng_sol.pdf)
- **Vorlesungsfolien (525 Seiten):** [`Vorlesung/MWE_2026_2027_Slides.pdf`](./Vorlesung/MWE_2026_2027_Slides.pdf)

---

## 1. Prüfungsformat & Erkenntnisse aus der Altklausur (`MWE_WS2223_v1_eng_sol.pdf`)
- **Dauer:** 120 Minuten, nominal 83,5–100 Credits.
- **Zweiteilung:**
  1. **Part 1 (~40–50 % der Punkte): Prüfungs-Paper** (wird ca. 4 Wochen vor der Klausur auf ILIAS bekanntgegeben und liegt der Klausur bei). Kombination aus gezielten Verständnisfragen (1–3 Credits), Ersatzschaltbild-Skizze (3 Credits) und 2 Einsetz-Rechenaufgaben (je 6–6,5 Credits).
  2. **Part 2 (~50–60 % der Punkte): Allgemeine Vorlesungsaufgaben** zu Großsignal-Verstärkerkenngrößen ($\text{IP}_{\text{1dB}}, \text{OP}_{\text{1dB}}, P_{\text{sat}}, \text{IM}_3, \text{OIP}_3, \text{PAE}$), Zweielement-Impedanzanpassung im Smith-Diagramm (LC-Matching, Stubs, $\lambda/4$-Trafo, Bode-Fano-Kriterium / Konstant-$Q$-Kreise), LNA-Entwurf (Friis-Formel, Rauschkreise, induktive Source-Degeneration) und Halbleitertechnologien.
- **Wichtige Bewertungsregeln:**
  - Bei Rechenaufgaben gibt jeder korrekt in die Gleichung eingesetzte Wert **$0{,}5\,\text{Credits}$**, das Endergebnis mit Einheit **$3\,\text{Credits}$**, und jede falsche/fehlende Einheit führt zu **$-0{,}25\,\text{Credits}$ Abzug**!
  - Jeder aus dem Paper/Datenblatt abgelesene Wert muss **sowohl auf dem Lösungsblatt als auch direkt im Paper/Datenblatt** markiert und beschriftet werden (*„Value for task X.Y“*).

## 2. Wichtigste Stolpersteine
- **Normierte vs. absolute Größen ($\text{A/mm}$ vs. $\text{A}$ und $\Omega\cdot\text{mm}$ vs. $\Omega$):** In $R_p = \frac{\beta(V_{\text{D,supply}} - V_k)}{I_{\max}'\,[\text{A/mm}]}$ hat das Ergebnis die Einheit **$\Omega\cdot\text{mm}$**!
- **Smith-Diagramm-Richtungen:** Serien-$L$ (Konstant-$R$-Kreis im Uhrzeigersinn nach oben), Serien-$C$ (Konstant-$R$-Kreis gegen den Uhrzeigersinn nach unten), Shunt-$C$ (Konstant-$G$-Kreis im Uhrzeigersinn nach unten $\leftrightarrow$ ersetzbar durch **Open Stub**), Shunt-$L$ (Konstant-$G$-Kreis gegen den Uhrzeigersinn nach oben $\leftrightarrow$ ersetzbar durch **Shorted Stub**).
- **Folie 69 (Kapitel 2.5 „Markets and Costs“):** Trägt im Vorlesungsskript den Vermerk **„Kommt nicht dran!!!“**.

