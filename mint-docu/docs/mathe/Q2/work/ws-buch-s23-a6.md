# Seite 23 Übung 6: Münzwerte bestimmen mit einem LGS

Es gibt 3 große (G), 16 mittlere (M) und 40 kleine (K) Münzen im Gesamtwert von 30€. Die Aufteilung ist „gerecht“ ⇒ jeder erhält **den gleichen Wert** (10€).  
Robert: 2G und 30K → Wert $= 10$  
Alfons: 8M und 10K → Wert $= 10$  
Edel: Rest (1G, 8M, 0K) → Wert $= 10$

Gesucht: die Münzwerte $g, m, k$ (in Euro).

## Lineares Gleichungssystem aufstellen

Aus den drei „Wert = 10“-Bedingungen ergeben sich:

$$
\begin{aligned}
\text{(R)}\quad & 2g \;+\; 30k \;=\; 10 \\
\text{(A)}\quad & 8m \;+\; 10k \;=\; 10 \\
\text{(E)}\quad & g \;+\; 8m \;=\; 10
\end{aligned}
$$

(Das Gesamtwert-Gleichgewicht $3g+16m+40k=30$ ist automatisch erfüllt, wenn alle drei Personen je 10€ erhalten.)

## Gaußscher Eliminationsalgorithmus

Schreibe das LGS als augmentierte Matrix (Reihenfolge der Unbekannten: $g, m, k$):

$$
\begin{pmatrix}
2 & 0 & 30 & \mid & 10 \\
0 & 8 & 10 & \mid & 10 \\
1 & 8 & 0  & \mid & 10
\end{pmatrix}
$$

1.  **Pivot 1 in Zeile 1 herstellen** (tausche $Z_1 \leftrightarrow Z_3$):

$$
\begin{pmatrix}
1 & 8 & 0  & \mid & 10 \\
0 & 8 & 10 & \mid & 10 \\
2 & 0 & 30 & \mid & 10
\end{pmatrix}
$$

2.  **Unter dem ersten Pivot eliminieren** ($Z_3 \leftarrow Z_3 - 2Z_1$):

$$
\begin{pmatrix}
1 & 8 & 0  & \mid & 10 \\
0 & 8 & 10 & \mid & 10 \\
0 & -16 & 30 & \mid & -10
\end{pmatrix}
$$

3.  **Unter dem zweiten Pivot eliminieren** ($Z_3 \leftarrow Z_3 + 2Z_2$):

$$
\begin{pmatrix}
1 & 8 & 0  & \mid & 10 \\
0 & 8 & 10 & \mid & 10 \\
0 & 0 & 50 & \mid & 10
\end{pmatrix}
$$

Nun Rückwärtseinsetzen:

*   Aus der 3. Zeile: $50k = 10 \Rightarrow k = 0{,}2$€.
*   Aus der 2. Zeile: $8m + 10k = 10 \Rightarrow 8m + 2 = 10 \Rightarrow m = 1$€.
*   Aus der 1. Zeile: $g + 8m = 10 \Rightarrow g + 8 = 10 \Rightarrow g = 2$€.

## Ergebnis (Münzwerte)

*   **Große Münze:** $g = 2{,}00$€
*   **Mittlere Münze:** $m = 1{,}00$€
*   **Kleine Münze:** $k = 0{,}20$€

**Probe:**

*   Gesamt: $3\cdot2 + 16\cdot1 + 40\cdot0{,}2 = 6 + 16 + 8 = 30$€ ✅
*   Robert: $2\cdot2 + 30\cdot0{,}2 = 4 + 6 = 10$€ ✅
*   Alfons: $8\cdot1 + 10\cdot0{,}2 = 8 + 2 = 10$€ ✅
*   Edel: $1\cdot2 + 8\cdot1 = 2 + 8 = 10$€ ✅

