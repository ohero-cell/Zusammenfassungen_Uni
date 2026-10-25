# Advanced Optical Fiber Communication (`AOFC`) – Lernstrategie & Übersicht

- **Haupt-Lernstrategie (alle 4 Fächer):** [`../Readme.md`](../Readme.md)
- **Ausführliche Formelsammlung (PDF, 26 Seiten):** [`Formelsammlung_Advanced_Optical_Fiber_Communication.pdf`](./Formelsammlung_Advanced_Optical_Fiber_Communication.pdf) (auch im Hauptverzeichnis [`../Formelsammlung_Advanced_Optical_Fiber_Communication.pdf`](../Formelsammlung_Advanced_Optical_Fiber_Communication.pdf))
- **Realistische Probeklausur inkl. Musterlösung (PDF):** [`Probeklausur_Advanced_Optical_Fiber_Communication.pdf`](./Probeklausur_Advanced_Optical_Fiber_Communication.pdf) (auch im Hauptverzeichnis [`../Probeklausur_Advanced_Optical_Fiber_Communication.pdf`](../Probeklausur_Advanced_Optical_Fiber_Communication.pdf))
- **Vorlesungsfolien (Lectures 1–15 inkl. Quiz in Lecture 15):** [`Vorlesung/Slides/`](./Vorlesung/Slides/)
- **24 Übungsaufgaben (`Problem 1`–`24`) & Notizen:** [`Übungen/Advanced Optical Fiber Communications - Exercise(1)/`](./Übungen/Advanced%20Optical%20Fiber%20Communications%20-%20Exercise(1)/)

---

## 1. Prüfungsformat & Konkreter Lernfahrplan
- **6 zentrale Aufgaben-Archetypen aus `Problem 1` bis `Problem 24`:**
  1. **Ebene Wellen, Sellmeier & Grenzflächen (`Problem 1–7`):** Komplexer Wellenwiderstand $\underline{Z}$, Gruppenindex $N = n - \lambda\frac{dn}{d\lambda}$ aus Sellmeier-Gleichung, Regensensor mit Totalreflexion ($\varphi_c$), Fresnel-Gleichungen ($R_s, R_p$) und Brewster-Winkel ($\varphi_B$).
  2. **Stufenindex- & Gradientenindex-Fasern (`Problem 9–11`):** $V$-Parameter, Ablesen von $B$, $\frac{d(VB)}{dV}$ und $V\frac{d^2(VB)}{dV^2}$ aus den Diagrammen für $n_{\text{eff}}$, Gruppenlaufzeit $\tau$, DMD $\Delta t$ und Zero-Dispersion-Design ($D_M + D_W = 0$); Modengruppen $\text{MG} = l + 2p - 1$ ($2l + 4p = \text{const.}$) in Parabolprofil-Fasern.
  3. **Gauß-Pulsverbreiterung & Chirp (`Problem 12`):** $T_{\text{FWHM}} = 1{,}665\,T_0$, $\sigma_0 = T_{\text{FWHM}}/2{,}355$, $\sigma_{\text{tot}} = \sqrt{\sigma_0^2 + (|D|\sigma_\lambda L)^2}$, Verbreiterungsfaktor gechirpter Pulse und Bitratenlimit $B_{\max} = \frac{1}{4\sigma_{\text{tot}}}$.
  4. **Faserkopplung, MZM & PIN-Photodiode (`Problem 13–15`):** Marcuse-Formel ($w/a$), Confinement $\Gamma = 1 - e^{-2a^2/w^2}$, Butt-Coupling $\eta(\Delta x)$; asymmetrischer MZM ($p = P_1/P_2$, Extinction Ratio $\text{ER}$, Pockels-Halbwellenspannung $U_\pi$); InGaAs/InP-PIN-Photodiode ($\lambda_g = hc_0/E_g$, Responsivität $R$, $3\,\text{dB}$-Bandbreite).
  5. **Kohärenter $90^\circ$-Hybrid, EDFA & OSNR-Link-Budget (`Problem 16–18`, `21`):** Balanced Detection ($I_I, I_Q$), EDFA-Gewinn & Rauschzahl ($F_{\text{amp}} \approx 2n_{\text{sp}}$), Friis-Kaskade und die $58\,\text{dB}$-OSNR-Formel.
  6. **DP-$M$-QAM, CD-FIR-Filter-Taps & SDM/MIMO (`Problem 18`, `21`, `22`):** $R_b = \frac{2 R_s \log_2 M}{1 + \text{OH}}$, $\text{OSNR}_{[\text{dB}]} = \text{SNR}_{[\text{dB}]} + 10\log_{10}(\Delta f / 12{,}5\,\text{GHz})$, quadratische Skalierung $N_{\text{taps}} \propto |\text{CD}_{\text{res}}| \cdot R_s^2$, MIMO-Shannon-Kapazität über Eigenwerte von $\mathbf{H}\mathbf{H}^T$ und Zero-Forcing $\hat{\mathbf{x}} = \mathbf{H}^{-1}\mathbf{y}$.

## 2. Wichtigste Stolpersteine (inkl. Tippfehler in `AOFC_formulary_updated.pdf`)
- **Tippfehler im Vorab-Formulary beachten (siehe Block 12 der Formelsammlung):** Unter der Wurzel von $d_{\text{eva}}$ (Gl. 13) muss $\sin^2\varphi$ stehen; in der Marcuse-Formel (Gl. 27) steht links $w/a$ (Spot-Radius $w$, nicht $\omega$); in Gl. (35) lautet die empirische Formel $D_M(\lambda) \approx 122(1 - \lambda_{\text{ZD}}/\lambda)\,\text{ps/(nm}\cdot\text{km)}$.
- **Zero-Dispersion-Design (`Problem 10d`):** Im Diagramm $V\frac{d^2(VB)}{dV^2}$ immer den **größeren Schnittpunkt $V > 1{,}15$** (z. B. $V = 1{,}45$ statt $0{,}8$) wählen, da für $V < 1$ keine brauchbare Kernführung vorliegt!
- **Feld-Dämpfung vs. Leistungs-Dämpfung:** $\alpha_{\text{dB}} = 8{,}686\,\alpha_{\text{Feld}} = 4{,}343\,\alpha_p$.

