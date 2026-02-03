# Der Gaußsche Algorithmus zur Lösung von linearen Gleichungssystemen (LGS)

## 🚀 Einfache Anleitung: Gaußscher Algorithmus für 3 Variablen

Ziel des Verfahrens:  
Ein lineares Gleichungssystem schrittweise so umformen, dass man am Ende durch **Rückwärtseinsetzen** leicht $z$, dann $y$, dann $x$ bestimmen kann.

## 1. Schritt: Gleichungssystem als Matrix schreiben

Aus dem System

$$
\begin{cases}
a_1x + b_1y + c_1z = d_1 \\
a_2x + b_2y + c_2z = d_2 \\
a_3x + b_3y + c_3z = d_3  
\end{cases}
$$

machst du die erweiterte Matrix:

$$
\left[
\begin{array}{ccc|c}
a_1 & b_1 & c_1 & d_1 \\
a_2 & b_2 & c_2 & d_2 \\
a_3 & b_3 & c_3 & d_3
\end{array}
\right]
$$

## 2. Schritt: Erste Spalte unterhalb des ersten Eintrags zu 0 machen

Mit Zeilenoperationen:

$Z_2 := Z_2 - k \cdot Z_1$

$Z_3 := Z_3 - m \cdot Z_1$

Damit erzeugst du:

$$
\begin{array}{cccc}
\text{Zeile 1:} & * & * & * & * \\
\text{Zeile 2:} & 0 & * & * & * \\
\text{Zeile 3:} & 0 & * & * & *
\end{array}
$$

## 3. Schritt: Zweite Spalte unterhalb des zweiten Eintrags zu 0 machen

Jetzt arbeitest du mit Zeile 2:

$Z_3 := Z_3 - k \cdot Z_2$

Du bekommst:

$$
\begin{array}{cccc}
\text{Zeile 1:} & * & * & * & * \\
\text{Zeile 2:} & 0 & * & * & * \\
\text{Zeile 3:} & 0 & 0 & * & *
\end{array}
$$

Die Matrix ist jetzt in **oberer Dreiecksform**.

## 4. Schritt: Rückwärtseinsetzen

Jetzt liest du ab:

### 🔹 Aus der letzten Zeile:

$$
c z = d \quad \Rightarrow \quad z = \frac{d}{c}
$$

### 🔹 In die zweite Zeile einsetzen:

$$
b y + c'z = d' \quad \Rightarrow \quad y \text{ ausrechnen}
$$

### 🔹 In die erste Zeile einsetzen:

$$
a x + b'y + c''z = d'' \quad \Rightarrow \quad x \text{ ausrechnen}
$$


## ✔️ Damit hast du die Lösung:

$$
(x,\; y,\; z)
$$

## Zusammenfassung in 5 Punkten

1.  Erweiterte Matrix aufstellen.
2.  Erste Spalte unterhalb von Zeile 1 auf 0 bringen.
3.  Zweite Spalte unterhalb von Zeile 2 auf 0 bringen.
4.  Dadurch entsteht eine obere Dreiecksmatrix.
5.  Von unten nach oben zurückrechnen: erst $z$, dann $y$, dann $x$.

