# Master-Semester Lernstrategie & Prüfungsleitfaden

Dieses Repository bündelt sämtliche Vorlesungsunterlagen, Übungsaufgaben, Zusatzmaterialien, Formelsammlungen (im PDF-Format) und Probeklausuren (im PDF-Format inkl. Musterlösungen) für die **vier Kernfächer des aktuellen Master-Semesters an der Universität Stuttgart**:

1. **Microwave Engineering (`MWE`)** – Prof. Dr.-Ing. Ingmar Kallfass (Institut für Robuste Leistungshalbleitersysteme – ILH)
2. **Radio Frequency Technology (`HF3` / Hochfrequenztechnik)** – Prof. Dr. Jan Hesselbarth (Institut für Hochfrequenztechnik – IHF)
3. **Introduction to CMOS Analog Integrated Circuit Design (`Intro_to_CMOS`)** – Prof. Dr.-Ing. Jens Anders / Dr. Nima Shahpari (Institut für Intelligente Sensorik und Theoretische Elektrotechnik – IIS)
4. **Advanced Optical Fiber Communication (`AOFC`)** – Prof. Dr.-Ing. Georg Rademacher / Julian Schneck (Institut für Elektrische und Optische Nachrichtentechnik – INT)

---

## 1. Übersicht der Ordnerstruktur & Generierten Prüfungsunterlagen

| Fach | Vorhandene Originalunterlagen im Workspace | Neu erstellte Formelsammlung (PDF) | Neu erstellte Probeklausur inkl. Musterlösung (PDF) |
| :--- | :--- | :--- | :--- |
| **Microwave Engineering** | `Vorlesung/MWE_2026_2027_Slides.pdf` (525 Folien, Kap. 1–8), `old exams/MWE_WS2223_v1_eng_sol.pdf` (Altklausur WiSe 22/23 inkl. Musterlösung) | `Formelsammlung_Microwave_Engineering.pdf` (38 Seiten) | `Probeklausur_Microwave_Engineering.pdf` |
| **HF3 (Radio Frequency Technology)** | `Vorlesung/RFT (HF3).pdf` (122 Seiten Hauptskript), `HF_1_altes_damaligen_material.pdf` (134 Seiten Grundlagen), `Übungen/` (12 Übungsblätter `RFT_exercise_1` bis `12` + `Materials_extra/` mit Smith-Chart, Microstrip-Basics, Hohlleitertabellen) | `Formelsammlung_HF3.pdf` (42 Seiten) | `Probeklausur_HF3.pdf` |
| **Intro to CMOS Analog IC Design** | `Vorlesung/Presentation Files/` (`Introduction` + `Chapter 01` bis `Chapter 06`, 359 Folien), `Übungen/` (`Ex1` bis `Ex7` inkl. Teilblättern `Ex1-2`, `Ex4-2`, `Ex4-3`, 204 Seiten) | `Formelsammlung_Intro_to_CMOS.pdf` (45 Seiten) | `Probeklausur_Intro_to_CMOS.pdf` |
| **Advanced Optical Fiber Communication** | `Vorlesung/Slides/` (Lectures 1–15 inkl. annotierter Folien), `Übungen/` (`Problems/` mit `Problem 1` bis `24`, `Notes/` mit 13 handschriftlichen Musterlösungen, `Slides/` Übungsfolien 1–6, `AOFC_formulary_updated.pdf`) | `Formelsammlung_Advanced_Optical_Fiber_Communication.pdf` (26 Seiten) | `Probeklausur_Advanced_Optical_Fiber_Communication.pdf` |

*(Alle PDF-Formelsammlungen und PDF-Probeklausuren liegen sowohl im Hauptverzeichnis als auch im jeweiligen Fach-Unterordner.)*

---

## 2. Analyse der vorhandenen Altklausur (`MWE_WS2223_v1_eng_sol.pdf`) – Wie sehen die Prüfungsanforderungen typischerweise aus?

Aus der im Ordner `Microwave_Engineering/old exams/MWE_WS2223_v1_eng_sol.pdf` vorliegenden Originalklausur mit Musterlösung und Korrekturmaßstab lassen sich entscheidende Erkenntnisse über den Klausurstil ableiten:

### A. Formale Rahmenbedingungen & Punktevergabe
- **Prüfungsdauer & Umfang:** **120 Minuten**, ausgelegt auf nominal **83,5 bis 100 Credits** (also knapp $1\,\text{Credit}$ pro Minute Bearbeitungszeit).
- **Zweigeteilter Klausuraufbau (speziell bei MWE, übertragbar als Mix aus Theorie/Transfer und Standardaufgaben):**
  - **Teil 1 (~40–50 % der Punkte): Transfer- & Paper-Aufgabe (`Task 1 – 39.5 Credits`, 15 Unterpunkte):** Bezieht sich auf ein ca. 4 Wochen vor der Klausur bekanntgegebenes IEEE-Paper (in WiSe 22/23: *C. F. Campbell, „Evolution of the Nonuniform Distributed Power Amplifier“, IEEE Microwave Magazine, 2019*). Dieser Teil kombiniert kurze Konzeptfragen (je $1\text{–}3\,\text{Credits}$) mit zwei gezielten Einsetz-Rechenaufgaben (je $6\text{–}6{,}5\,\text{Credits}$) und einer Ersatzschaltbild-Zeichenaufgabe ($3\,\text{Credits}$).
  - **Teil 2 (~50–60 % der Punkte): Allgemeine Vorlesungsaufgaben (`Task 2 – 20 Credits` & `Task 3 – 24 Credits`):**
    - `Task 2`: Großsignal-Messkurven eines Leistungsverstärkers ($P_{\text{out}}$ über $P_{\text{in}}$ und $G$ über $P_{\text{in}}$) interpretieren ($\text{IP}_{\text{1dB}}, \text{OP}_{\text{1dB}}, P_{\text{sat}}, G_0, G_{\text{1dB}}$), Umrechnungsformel $\text{OP}_{\text{1dB}} = \text{IP}_{\text{1dB}} + G_{\text{1dB}}$, Vergleich Radar ($P_{\text{sat}}$) vs. Kommunikation ($\text{P}_{\text{1dB}}$), Zweiton-Anregung, $\text{IM}_3$-Intermodulation und $\text{OIP}_3$.
    - `Task 3`: Smith-Diagramm-Anpassung (2-Element-L-Glied von $Z_{\text{out}}$ nach $Z_{\text{goal}}$): Aus gegebenem Pfad das LC-Schaltbild (Serien-$L$, Shunt-$C$) zeichnen, für das duale Schaltbild (Serien-$C$, Shunt-$L$) den Pfad ins Smith-Diagramm einzeichnen, Ersetzen von konzentrierten Elementen durch Stubs/Übertragungsleitungen bei Millimeterwellen, $\lambda/4$-Transformator und Vergleich der Bandbreite über das **Bode-Fano-Kriterium** (Kurven konstanter Güte $Q$ im Smith-Diagramm).
- **Exakter Korrektur- und Punktemaßstab aus der Musterlösung:**
  - **Stichwort-Prinzip bei Verständnisfragen:** Jedes geforderte Schlüsselkonzept gibt exakt **$1\,\text{Credit}$** (z. B. *„high output power 1, power handling 1“* oder *„IM3 product 1, close to the carrier 1, OIP3 1“*). Es werden keine langen Aufsätze erwartet, sondern präzise Fachbegriffe!
  - **Bewertung von Rechenaufgaben (6–6,5 Credits):**
    - **$0{,}5\,\text{Credits}$ für jeden korrekt in die Formel eingesetzten Zahlenwert** (auch wenn man sich am Ende im Taschenrechner vertippt, sichert das saubere Aufschreiben der eingesetzten Zahlenwerte bereits über $50\,\%$ der Punkte!).
    - **$3\,\text{Credits}$ für das richtige Endergebnis inkl. korrekter Einheit** (z. B. $\text{GHz}$ bzw. $\Omega\cdot\text{mm}$).
    - **$-0{,}25\,\text{Credits}$ Punktabzug für jede falsche oder fehlende Einheit!**
  - **Strenge Datenblatt-/Paper-Regel (Deckblatt Punkt 6):** Jeder Wert, der aus einem beigefügten Paper oder Datenblatt abgelesen wird, muss **sowohl auf dem Lösungsbogen** (*„Value from page X of data sheet“*) **als auch im Datenblatt selbst** (*Wert einkreisen + „Value for task X.Y“*) markiert werden!

---

## 3. Fachspezifische Lernstrategien & Stolpersteine

---

### Fach 1: Microwave Engineering (`MWE`)

#### A. Was muss ich konkret tun, um das Fach zu bestehen?
1. **Prüfungs-Paper (4 Wochen vor der Klausur auf ILIAS) intensiv durcharbeiten:**
   - Da **Teil 1 fast die Hälfte der Gesamtpunkte (~40 Credits)** ausmacht, ist die gründliche Vorbereitung des ausgegebenen Papers der größte Hebel zum sicheren Bestehen.
   - Markiere vorab im Verständnis alle Gleichungen im Paper (wie die Bode-Fano-Gleichung $\text{BW} < \frac{4{,}343 I_{\max}}{\text{RL}_{\text{dB}} C_p \beta (V_{\text{D,supply}} - V_{\text{knee}})}$ und den Norton-Widerstand $R_p = \frac{\beta(V_{\text{D,supply}} - V_{\text{knee}})}{I_{\max}}$ im Campbell-Paper), alle Ersatzschaltbilder und alle im Paper verglichenen Topologien (z. B. Uniform DA vs. NDPA, Ruthroff-/Trifilar-/$\lambda/4$-Transformatoren).
2. **Smith-Diagramm & 2-Element-Matching im Schlaf beherrschen (Kapitel 3, garantiert ~20–25 Credits):**
   - Übe den Wechsel zwischen **Schaltbild $\leftrightarrow$ Pfad im Smith-Diagramm** für alle 4 Kombinationen aus Serien-$L$, Serien-$C$, Shunt-$L$ und Shunt-$C$:
     - **Serien-$L$:** Auf Konstant-$R$-Kreis im Uhrzeigersinn nach **oben** (induktive Halbebene).
     - **Serien-$C$:** Auf Konstant-$R$-Kreis gegen den Uhrzeigersinn nach **unten** (kapazitive Halbebene).
     - **Shunt-$C$:** Auf Konstant-$G$-Kreis (Admittanzkreise, nach links geöffnet) im Uhrzeigersinn nach **unten**.
     - **Shunt-$L$:** Auf Konstant-$G$-Kreis gegen den Uhrzeigersinn nach **oben**.
   - Merke dir die Millimeterwellen-Äquivalente: **Shunt-$C \leftrightarrow$ Open Stub** ($l < \lambda'/4$), **Shunt-$L \leftrightarrow$ Shorted Stub** ($l < \lambda'/4$), **Serien-$L \leftrightarrow$ kurzes hochohmiges Leitungsstück (Transmission Line)**, reelle Impedanztransformation mit 1 Element $\leftrightarrow$ **$\lambda/4$-Transformator** ($Z_T = \sqrt{Z_0 R_L}$).
3. **Leistungsverstärker (PA) & Nichtlinearität lernen (Kapitel 6, garantiert ~20 Credits):**
   - Verinnerliche die Großsignal-Kennlinien ($P_{\text{out}}$ und $G$ über $P_{\text{in}}$), Einton- vs. Zweiton-Anregung, $\text{IP}_{\text{1dB}}, \text{OP}_{\text{1dB}} = \text{IP}_{\text{1dB}} + G_0 - 1\,\text{dB}$, $P_{\text{sat}}$, $\eta_D$, $\text{PAE} = \eta_D(1 - 1/G)$, $\text{IM}_3$ bei $2\omega_1 - \omega_2$ und $2\omega_2 - \omega_1$, $\text{OIP}_3 = P_{\text{out}} + \Delta P / 2$, $\text{SFDR}$, Cripps-Lastgerade $R_{\text{opt}} = \frac{V_{\max}-V_{\text{knee}}}{I_{\max}}$, Load-Pull und Verstärkerklassen (A, AB, B, C, E, F, Doherty).
4. **LNA, Breitbandverstärker & Halbleitertechnologien wiederholen (Kapitel 2, 4, 5):**
   - Halbleitervergleich (GaN auf SiC: hohe Durchbruchspannung & Ausgangsleistung, hohe Wärmeleitfähigkeit von SiC; InP HEMT: höchste $f_T/f_{\max}$ und niedrigstes $\text{NF}_{\min}$; SiGe HBT: niedriges $1/f$-Rauschen für VCOs, hohe Steilheit $g_m$; Si CMOS: höchste Integrationsdichte).
   - *Hinweis aus Folie 69 des Skripts:* Kapitel 2.5 („Markets and Costs“) trägt im Skript den roten Vermerk **„Kommt nicht dran!!!“** – hier keine Lernzeit verschwenden!
   - LNA: Friis-Formel, Noise Measure $M$, Rauschkreise vs. Verstärkungskreise und **induktive Source-Degeneration $L_s$** ($Z_{\text{in}} \approx 2\pi f_T L_s - j\frac{1}{\omega C_{gs}}$ erzeugt einen rauschfreien Realteil am Eingang, um $\Gamma_{\text{opt}}$ und $\Gamma_{\text{in}}^*$ zusammenzuführen!).
   - Breitbandverstärker: Induktives Shunt-Peaking, Shunt-Feedback/TIA, Kaskode (Vermeidung des Miller-Effekts, negativ werdender Ausgangswiderstand bei hohen Frequenzen) und Wanderwellenverstärker (TWA / NDPA).

#### B. Häufigste Stolpersteine in MWE
- **Flächen-/Weiten-Normierung bei MMIC-Transistoren ($\text{A/mm}$ und $\Omega\cdot\text{mm}$):** In MMIC-Prozessen wird der Maximalstrom oft auf die gesamte Gateweite (TGW) normiert angegeben (z. B. $I_{\max}' = 1\,\text{A/mm}$ bzw. in der Altklausur $1000\,\text{A/mm}$). Setzt man den normierten Strom in $R_p = \frac{\beta(V_{\text{D,supply}} - V_k)}{I_{\max}'}$ ein, hat das Ergebnis die Einheit **$\Omega\cdot\text{mm}$** (nicht $\Omega$!). Um auf den absoluten Widerstand in $\Omega$ zu kommen, muss man durch die Gateweite in $\text{mm}$ teilen!
- **Einheiten in der Bode-Fano-PA-Formel:** In $\text{BW} < \frac{4{,}343 I_{\max}}{\text{RL}_{\text{dB}} C_p \beta (V_{\text{D,supply}} - V_{\text{knee}})}$ wird $\text{RL}_{\text{dB}}$ direkt als positiver Zahlenwert in $\text{dB}$ (z. B. $20$ für $20\,\text{dB}$ Return Loss) eingesetzt, weil der Umrechnungsfaktor $20 / \ln(10) \approx 8{,}686$ (bzw. $10/\ln(10) = 4{,}343$) bereits im Vorfaktor $4{,}343$ steckt! $C_p$ muss in $\text{F}$ ($1\,\text{pF} = 10^{-12}\,\text{F}$) eingesetzt werden, damit $\text{BW}$ in $\text{Hz}$ ($10^9\,\text{Hz} = 1\,\text{GHz}$) herauskommt.
- **Bandbreite dualer L-Glieder:** Ob man von $Z_{\text{out}}$ nach $Z_{\text{goal}}$ über den oberen Pfad (Serien-$L$ + Shunt-$C$, Tiefpass) oder den unteren Pfad (Serien-$C$ + Shunt-$L$, Hochpass) geht – beide berühren im Umkehrpunkt exakt dieselbe **Konstant-$Q$-Kontur** im Smith-Diagramm und haben daher nach Bode-Fano **dieselbe relative Anpassbandbreite**!

---

### Fach 2: Radio Frequency Technology (`HF3` / Hochfrequenztechnik)

#### A. Was muss ich konkret tun, um das Fach zu bestehen?
1. **Open-Book-Vorteil optimal nutzen:**
   - In der 120-minütigen Klausur bei Prof. Hesselbarth sind **alle gedruckten und handschriftlichen Unterlagen erlaubt**. Drucke dir `Formelsammlung_HF3.pdf`, `Probeklausur_HF3.pdf`, die 12 Übungsblätter sowie ein paar leere `SmithChart.pdf`-Bögen und die Hohlleiter-/Modentabellen aus und versehe die 11 Blöcke der Formelsammlung mit Kleberegistern (Tabs).
2. **Die 12 Übungsblätter (`RFT_exercise_1` bis `12`) aktiv durchrechnen:**
   - Die Klausur orientiert sich extrem eng an den 12 Übungsblättern. Arbeite sie in 5 thematischen Paketen durch:
     - **Paket 1 (Übung 1–3): S-Parameter, Leitungen, Smith-Chart, Microstrip & Stripline:** Unitarität ($[S]^H[S] = [E]$), Eingangsreflexionsfaktor $\Gamma_{\text{in}} = S_{11} + \frac{S_{12}S_{21}\Gamma_L}{1 - S_{22}\Gamma_L}$, verlustbehaftete Leitungen mit $\cosh/\sinh(\gamma l)$, Stichleitungsanpassung im Smith-Chart, Wheeler-Formeln für Microstrip und Stripline-Leistungsteiler.
     - **Paket 2 (Übung 4–6): Rechteckhohlleiter:** Modenidentifikation aus Feldgleichungen, Grenzfrequenz $f_{c,mn} = \frac{c}{2\pi}\sqrt{(m\pi/a)^2 + (n\pi/b)^2}$, Cutoff-Dämpfungsglied ($\alpha_{\text{evan}} = \sqrt{k_c^2 - k^2}$), Leistungsfluss $P_{\text{TE}_{10}} = \frac{ab}{4Z_{\text{TE}}}E_{\max}^2$, Wandverluste $\alpha_c$ und selektive Sonden-/Schlitzanregung.
     - **Paket 3 (Übung 7–8): Rundhohlleiter, Koaxialkabel & Dielektrische Filmwellenleiter (Slab Waveguides):** Bessel-Nullstellen $p_{mn}$ ($\text{TM}$) und $p'_{mn}$ ($\text{TE}$), Modenreihenfolge ($\text{TE}_{11} \to \text{TM}_{01} \to \text{TE}_{21} \to \text{TE}_{01}/\text{TM}_{11}$), koaxiale $\text{TM}_{01}$-Anregung, Mehrwege-Gruppenlaufzeitdifferenz und Oberflächenwellen ($\text{TM}_0$ ohne Cutoff auf Grounded Slab!).
     - **Paket 4 (Übung 9–10): Mikrowellen- & Hohlraumresonatoren:** Verkürzter $\lambda/4$-Koaxialresonator mit Endkapazität ($\frac{1}{\omega_0 C_K} = Z_0\tan(\beta l)$), Rechteck- ($\text{TE}_{101}, \text{TM}_{110}$) und Zylinderresonatoren ($\text{TM}_{010}$ mit $f_r \approx \frac{c_0}{1{,}31 D}$, $\text{TE}_{011}$ mit maximalem $Q$ bei $D = h$), unbelastete/belastete/externe Güte ($\frac{1}{Q_L} = \frac{1}{Q_0} + \frac{1}{Q_{\text{ext}}}$, $|S_{21}(f_r)| = 1 - \frac{Q_L}{Q_0}$ bei symmetrischer Transmissionskopplung) und Materialwechsel ($Q_{\text{cond}} \propto \sqrt{\sigma}$).
     - **Paket 5 (Übung 11–12): Ferrite, Phasenrauschen & VNA:** Larmor-Frequenz $f_0 = 2{,}8\,\text{MHz/Oe}\cdot H_0$, Magnetisierungsfrequenz $f_m = 2{,}8\,\text{MHz/G}\cdot (4\pi M_s)$, $\mu_\pm$ für RHCP/LHCP, Faraday-Drehung $\theta = \frac{\beta_+ - \beta_-}{2}z$, Leeson-Formel für Oszillator-Phasenrauschen und OSM-Kalibrationsrestfehler beim VNA.
3. **Die „Short Questions“ am Ende der Übungsblätter 5–12 gezielt wiederholen:**
   - Prof. Hesselbarth stellt in jeder Klausur konzeptionelle Kurzfragen (Skizzieren von Feldlinien, Platzieren von Stiftsonden/Koppelschleifen/Schlitzen, Abschätzen von Frequenzverschiebungen ohne Taschenrechner). Alle diese Kurzfragen und ihre Musterantworten sind in `Formelsammlung_HF3.pdf` integriert!

#### B. Häufigste Stolpersteine in HF3
- **$\text{Np/m}$ vs. $\text{dB/m}$ bei Dämpfungsbelägen $\alpha$:** Alle physikalischen Formeln für Leiter- und Dielektrikumsdämpfung ($\alpha_c, \alpha_d$) sowie $\gamma = \alpha + j\beta$ in $\sinh(\gamma l), \cosh(\gamma l), e^{-\alpha l}$ und $Q_0 = \frac{\beta}{2\alpha}$ arbeiten zwingend in **$\text{Np/m}$**! Ist $\alpha$ in $\text{dB/m}$ gegeben (wie in Übung 2.1 oder 6.2), muss sofort durch **$8{,}6859$** geteilt werden ($\alpha_{[\text{Np/m}]} = \alpha_{[\text{dB/m}]} / 8{,}6859$).
- **Spitzenwert vs. Effektivwert im Poynting-Vektor:** In $P_{\text{TE}_{10}} = \frac{ab}{4Z_{\text{TE}}}E_{\max}^2$ ist $E_{\max}$ der **zeitliche Spitzenwert (Peak)** der Feldstärke am Ort des Maximums ($x = a/2$).
- **Entartung von $\text{TE}_{01}$ und $\text{TM}_{11}$ im Rundhohlleiter (und $\text{TE}_{011}/\text{TM}_{111}$ im Zylinderresonator):** Wegen der Bessel-Identität $J'_0(x) = -J_1(x)$ ist $p'_{01} = p_{11} = 3{,}8317$. Beide Moden haben exakt dieselbe Grenzfrequenz und dieselbe Gruppengeschwindigkeit!
- **Invarianz von $\text{TM}_{mn0}$-Resonatoren bezüglich der Höhe/Länge:** Bei $\text{TM}_{110}$ (Rechteck) und $\text{TM}_{010}$ (Zylinder) ist die longitudinale Indexzahl $p = 0$ ($\beta_z = 0$). Die Resonanzfrequenz hängt **nur vom Querschnitt ($a, b$ bzw. $D$)** ab, nicht von der Länge $c$ bzw. Höhe $h$ (die Höhe $h$ beeinflusst nur die Güte $Q_0$!).

---

### Fach 3: Introduction to CMOS Analog Integrated Circuit Design (`Intro_to_CMOS`)

#### A. Was muss ich konkret tun, um das Fach zu bestehen?
1. **Dreistufiges Standard-Rechenschema für jede Schaltungsaufgabe automatisieren:**
   Fast jede Klausuraufgabe in `Intro_to_CMOS` folgt demselben Schema aus den Übungen `Ex1`–`Ex7`:
   - **Schritt 1 – DC-Arbeitspunkt & Dimensionierung (Großsignal):** Aus gegebenem Ruhestrom $I_D$ und geforderter Overdrive-Spannung $V_{GSeff} = V_{GS} - V_{th} = \sqrt{\frac{2 I_D}{\mu C'_{ox}(W/L)}}$ das Verhältnis $(W/L)$ (bzw. bei gegebenem $L$ die Weite $W$) berechnen und die Sättigungsbedingung $V_{DS} \ge V_{GSeff}$ (für NMOS) bzw. $V_{SD} \ge V_{SGeff} = V_{SG} - |V_{th,p}|$ (für PMOS) prüfen!
   - **Schritt 2 – Kleinsignalparameter am Arbeitspunkt berechnen:**
     $$g_m = \mu C'_{ox}\frac{W}{L}V_{GSeff} = \sqrt{2\mu C'_{ox}\frac{W}{L}I_D} = \frac{2 I_D}{V_{GSeff}}, \qquad g_{ds} = \frac{1}{r_{ds}} = \lambda I_D, \qquad g_{mb} = \eta g_m = \frac{\gamma}{2\sqrt{2\Phi_F + V_{SB}}}g_m$$
   - **Schritt 3 – Kleinsignalanalyse (Zweitor-Y-Parameter $G_m, r_{out}, A_v = -G_m r_{out}$) & Frequenzgang (Pole/Nullstellen):** Knotenkapazitäten (inkl. Miller-Kapazität) aufstellen und Pole $\omega_{p,i} = -\frac{1}{R_i C_i}$ sowie RHP-Nullstellen $\omega_z = +\frac{g_m}{C_{GD}}$ bestimmen.
2. **Die 7 Übungsblätter (`Ex1` bis `Ex7`) inklusive der Teilblätter (`Ex1-2`, `Ex4-2`, `Ex4-3`) lückenlos beherrschen:**
   - **`Ex1` & `Ex1-2`:** Parameterextraktion ($\lambda, V_{th}, \beta$) aus 4 Messpunkten eines Ausgangskennlinienfelds; Twin-Well-Querschnitt (NMOS-Bulk an $V_{SS}$, PMOS-n-Well an $V_{DD}$).
   - **`Ex2`:** Arbeitspunktabhängige MOSFET-Kapazitäten ($C_{GS}, C_{GD}$ in Cutoff, Linear [$0{,}5\,C_{ox}$] und Sättigung [$0{,}6\,C_{ox}$ bzw. $\frac{2}{3}C_{ox}$ + Überlappkapazität]); CMOS-Push-Pull-Inverter als Verstärker ($G_m = g_{m,n} + g_{m,p}$).
   - **`Ex3`:** Mehrstufige NMOS/PMOS-Stromspiegelketten MIT Kanallängenmodulation $\lambda$ dimensionieren ($\frac{(W/L)_2}{(W/L)_1} = \frac{I_{D2}}{I_{D1}}\frac{1 + \lambda V_{DS1}}{1 + \lambda V_{DS2}}$), optimaler Ausgangspunkt $V_{\text{OUT,opt}} = V_{GS1,2}$ und maximaler Lastwiderstand $R_{L,\text{max}}$.
   - **`Ex4`, `Ex4-2`, `Ex4-3`:** Rückwärts-Entwurf eines CS-Verstärkers aus gefordertem Gain $A_v$ und Ausgangs-Swing $\Delta v_{\text{OUT}}$; Geregelte Kaskode (Regulated Cascode / Gain-Boosting mit $r_{out} \approx A g_{m4} r_{ds4} r_{ds3}$); Source-Folger mit und ohne Body-Effekt ($A_v = \frac{g_{m1}R_L}{1 + (g_{m1}+g_{mb1})R_L}$).
   - **`Ex5`:** Bode-Diagramm, Unity-Gain-Frequenz $f_u$, Phasenreserve $\text{PM} = 180^\circ + \angle H_0(jf_u)$, invertierender OP mit endlicher Verstärkung $A_D(s)$ und Y-Parameter-Herleitung des CS-Frequenzgangs.
   - **`Ex6`:** Differenzstufe – Eingangs-Gleichtaktbereich ($\text{ICMR}$: $V_{CM,\text{in,min}}$ und $V_{CM,\text{in,max}}$) mit idealer Stromquelle, NMOS-Stromsenke, Kaskode-Stromsenke und **mit Body-Effekt**; Halbschaltungen für $A_{DM}, A_{CM}$ und $\text{CMRR} \approx 2 g_{m1} r_{ss}$.
   - **`Ex7`:** Symmetrischer mehrstufiger Current-Mirror-OTA – Zerlegung in nicht-invertierenden und invertierenden Signalpfad ($A_{DM} = \frac{A_p - A_n}{2}$) sowie Aufstellen aller Knotenkapazitäten, 4 Pole und 5 RHP-Nullstellen.

#### B. Häufigste Stolpersteine in Intro to CMOS
- **Zwei unterschiedliche Body-Effekt-Formeln in den Übungen:**
  - Ist in der Aufgabenstellung $2\Phi_F$ angegeben (wie in `Ex4` mit $2\Phi_F = 0{,}2\,\text{V}$), muss die **exakte Formel** $V_{th} = V_{th0} + \gamma\left(\sqrt{2\Phi_F + V_{SB}} - \sqrt{2\Phi_F}\right)$ verwendet werden.
  - Ist **kein** $2\Phi_F$ angegeben (wie in `Ex6` und `Chapter 06`), wird in der Musterlösung die **vereinfachte Formel** $V_{th} = V_{th0} + \gamma\sqrt{V_{SB}}$ genutzt!
- **Halber Ruhestrom pro Zweig in der Differenzstufe (`Ex6`, `Ex7`):** Die Fußpunkt-Stromquelle liefert $I_{SS}$, aber durch jeden der beiden Eingangstransistoren $M_1, M_2$ fließt im Gleichgewicht nur **$I_{D1} = I_{D2} = \frac{I_{SS}}{2}$**! Wer bei der Berechnung von $(W/L)_{1,2}$ oder $g_{m1,2}$ versehentlich $I_{SS}$ statt $I_{SS}/2$ einsetzt, liegt um den Faktor $2$ falsch.
- **Kaskode-Verstärker & Miller-Effekt (`Chapter 05` Folien 37–40):** Eine **einseitige** Kaskode (Kaskode unten + einfache PMOS-Stromquelle oben) unterdrückt den Miller-Effekt an $M_1$ fast vollständig, weil der Eingangswiderstand in den Source von $M_2$ niederohmig ist ($r_{in,S2} \approx \frac{2}{g_{m2}} \implies |A_{v1}| \approx 2\frac{g_{m1}}{g_{m2}}$ klein). Bei einer **Vollkaskode** (Kaskode unten + Kaskodenlast oben) transformiert die extrem hochohmige Kaskodenlast ($r_{out,P} \approx g_m r_{ds}^2$) den Eingangswiderstand von $M_2$ jedoch auf $r_{in,S2} \approx r_{ds1} \parallel r_{ds4}$ hoch, sodass $|A_{v1}|$ wieder groß wird und der Miller-Effekt an $C_{GD1}$ zurückkehrt!

---

### Fach 4: Advanced Optical Fiber Communication (`AOFC`)

#### A. Was muss ich konkret tun, um das Fach zu bestehen?
1. **Die 24 Übungsaufgaben (`Problem 1` bis `Problem 24`) zusammen mit der korrigierten Formelsammlung durchrechnen:**
   - In AOFC gibt es ein offizielles 4-seitiges Kurz-Formulary (`AOFC_formulary_updated.pdf`), das in der Klausur bereitgestellt bzw. genutzt wird, aber **mehrere gefährliche Tippfehler** enthält (alle in Block 12 von `Formelsammlung_Advanced_Optical_Fiber_Communication.pdf` dokumentiert!).
   - Beherrsche die **6 großen Rechen-Archetypen** der Übungen:
     1. **Wellenausbreitung, Sellmeier & Grenzflächen (`Problem 1–7`):** Komplexer Wellenwiderstand $\underline{Z}$, Gruppenindex $N = n - \lambda\frac{dn}{d\lambda}$ aus der Sellmeier-Gleichung, Regensensor mit Totalreflexion ($\varphi_c = \arcsin(n_2/n_1)$), Fresnel-Reflexion ($R_s, R_p$) und Brewster-Winkel ($\varphi_B = \arctan(n_2/n_1)$).
     2. **Stufenindex- & Gradientenindex-Fasern mit Diagramm-Ablesung (`Problem 9–11`):** $V = \frac{2\pi}{\lambda}a\sqrt{n_1^2 - n_2^2}$ berechnen $\to$ aus dem $B$-$V$-Diagramm (Formulary S. 4 oben) für alle ausbreitungsfähigen Moden $B$ ablesen $\to$ $n_{\text{eff}} = n_2 + B(n_1 - n_2)$ berechnen; aus dem $\frac{d(VB)}{dV}$-Diagramm die Gruppenlaufzeit $\tau = \frac{N_2}{c_0} + \frac{n_1 - n_2}{c_0}\frac{d(VB)}{dV}$ und DMD $\Delta t$ bestimmen; für Dispersionsnullstelle ($D = D_M + D_W = 0$) aus dem unteren Diagramm ($V\frac{d^2(VB)}{dV^2}$) den größeren Schnittpunkt $V \approx 1{,}45$ ablesen und den neuen Kernradius $a$ berechnen; Modengruppen $\text{MG} = l + 2p - 1$ ($2l + 4p = \text{const.}$) im Parabolprofil bestimmen.
     3. **Gauß-Pulsverbreiterung & Chirp (`Problem 12`):** Umrechnung $T_{\text{FWHM}} \leftrightarrow T_0 \leftrightarrow \sigma_0$, Berechnung von $\sigma_{\text{tot}} = \sqrt{\sigma_0^2 + (|D|\sigma_\lambda L)^2}$ für breitbandige Quellen ($\sigma_\lambda = \Delta\lambda_{\text{FWHM}}/2{,}355$) vs. kohärente Pulse ($\sigma_\lambda = \frac{\lambda^2}{4\pi c_0 \sigma_0}$), gechirpte Pulse mit $(1 + C\delta)^2 + \delta^2$ und maximale Bitrate $B_{\max} = \frac{1}{4\sigma_{\text{tot}}}$.
     4. **Faserkopplung, MZM-Modulator & PIN-Photodiode (`Problem 13–15`):** Marcuse-Formel für $w/a$, Confinement-Faktor $\Gamma = 1 - e^{-2a^2/w^2}$, Butt-Coupling-Effizienz $\eta(\Delta x)$; asymmetrischer MZM ($p = P_1/P_2$, Extinction Ratio $\text{ER}$, Halbwellenspannung $U_\pi$ über Pockels-Effekt in $\text{LiNbO}_3$); InGaAs/InP-PIN-Photodiode (Grenzwellenlängen aus $E_g$, Responsivität $R = \frac{\eta e \lambda}{hc_0}$, $3\,\text{dB}$-Bandbreite aus $\tau_{RC}$ und $\tau_n$).
     5. **Kohärenter $90^\circ$-Hybrid-Empfänger, EDFA & OSNR-Link-Budget (`Problem 16–18`, `21`):** Herleitung der 4 Ausgangsströme des $90^\circ$-Hybrids und der Differenzströme $I_I, I_Q$ bei Balanced Detection; EDFA-Gewinn und Rauschzahl $F_{\text{amp}} \approx 2 n_{\text{sp}}$, Friis-Kaskade $F_{\text{tot}} \approx N G F_{\text{amp}}$ und die **$58\,\text{dB}$-OSNR-Formel**:
        $$\text{OSNR}_{[\text{dB}]} = 58 + P_{0,[\text{dBm}]} - F_{\text{amp},[\text{dB}]} - \alpha_{\text{dB}} L_{\text{oa}} - 10\log_{10}(N)$$
     6. **DP-$M$-QAM-Systementwurf, CD-FIR-Filter-Taps & SDM/MIMO (`Problem 18`, `21`, `22`):** $R_b = \frac{2 R_s \log_2 M}{1 + \text{OH}}$, Umrechnung $\text{OSNR}_{[\text{dB}]} = \text{SNR}_{[\text{dB}]} + 10\log_{10}\left(\frac{\Delta f}{12{,}5\,\text{GHz}}\right)$, quadratische Skalierung der DSP-Filter-Taps $N_{\text{taps}} \propto |\text{CD}_{\text{res}}| \cdot R_s^2$, sowie MIMO-Shannon-Kapazität $C = 2\Delta f \sum \log_2(1 + \lambda_i\text{SNR})$ über die Eigenwerte $\lambda_i$ von $\mathbf{H}\mathbf{H}^T$ und Zero-Forcing-Entzerrung $\hat{\mathbf{x}} = \mathbf{H}^{-1}\mathbf{y}$.
2. **Die „Concept Tests“ und das Abschluss-Quiz (`Rademacher_AOFC_lecture_15_annotated.pdf`) durchgehen:**
   - Prof. Rademacher baut in fast jede Vorlesung Multiple-Choice-„Concept Tests“ ein und hat in **Vorlesung 15 ein komplettes Wiederholungs-Quiz** gehalten. Diese Fragen prüfen exakt das physikalische Verständnis, das in der Klausur abgefragt wird!

#### B. Häufigste Stolpersteine in AOFC
- **Faktor $2$ zwischen Feld-Dämpfung $\alpha_{\text{Feld}}$ und Leistungs-Dämpfung $\alpha_p$:** In $E(z) = E_0 e^{-\alpha_{\text{Feld}}z}$ fällt die Leistung mit $P(z) = P_0 e^{-2\alpha_{\text{Feld}}z}$ ab, sodass $\alpha_{\text{dB}} = 8{,}686\,\alpha_{\text{Feld}} = 4{,}343\,\alpha_p$ gilt!
- **Vorzeichenwechsel beim Gruppenindex $N$:** Als Funktion der Frequenz gilt $N(f) = n + f\frac{dn}{df}$ (**Plus!**), als Funktion der Wellenlänge gilt $N(\lambda) = n - \lambda\frac{dn}{d\lambda}$ (**Minus!**).
- **Wahl des richtigen $V$-Wertes beim Zero-Dispersion-Design (`Problem 10d`):** Die Kurve $V\frac{d^2(VB)}{dV^2}$ hat für Werte $< 1{,}46$ immer **zwei** Schnittpunkte ($V_1 < 1{,}15$ und $V_2 > 1{,}15$). Man muss immer den **rechten Schnittpunkt $V_2$** wählen, weil bei $V_1 < 1$ das Licht fast komplett im Mantel läuft ($B \approx 0$)!
- **Referenzbandbreite $\Delta f_{\text{ref}} = 12{,}5\,\text{GHz}$ beim OSNR:** Das optische $\text{OSNR}$ ist immer auf $12{,}5\,\text{GHz}$ ($0{,}1\,\text{nm}$) normiert, während das elektrische $\text{SNR}$ auf die tatsächliche Signalbandbreite $\Delta f \approx R_s$ bezogen ist. Bei $R_s = 28\,\text{GBd}$ liegt das benötigte $\text{OSNR}$ um $10\log_{10}(28 / 12{,}5) = +3{,}5\,\text{dB}$ höher als das elektrische $\text{SNR}_{\text{req}}$!

---

## 4. Empfohlener Zeitplan für die Klausurvorbereitung

1. **Phase 1 (Grundlagen & Formelsammlung verinnerlichen):** Arbeite für jedes Fach die jeweilige PDF-Formelsammlung (`Formelsammlung_[Fachname].pdf`) parallel zu den Vorlesungsfolien durch, sodass du sofort weißt, auf welcher Seite welche Formel steht und welche Einheiten eingesetzt werden müssen.
2. **Phase 2 (Übungsaufgaben selbstständig rechnen):** Rechne die Kernübungen jedes Fachs mithilfe der PDF-Formelsammlung ohne Blick in die Musterlösung durch (insb. die 12 HF3-Übungen, die 7 CMOS-Übungen und die 24 AOFC-Problems sowie das MWE-Prüfungspaper).
3. **Phase 3 (Generalprobe unter Echtzeitbedingungen):** Nimm dir für jedes Fach **exakt 120 Minuten** Zeit, drucke Teil I der jeweiligen **PDF-Probeklausur (`Probeklausur_[Fachname].pdf`)** aus, bearbeite sie nur mit den erlaubten Hilfsmitteln und korrigiere deine Lösung anschließend anhand des detaillierten **Teils II (Musterlösungen, Rechenwege & Punkteverteilung)** am Ende des jeweiligen PDFs.

