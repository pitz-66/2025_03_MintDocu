# Seite 19 Aufgabe 2a: Lösen eines linearen Gleichungssystems mit dem Gaußschen Eliminationsverfahren

## 🔢 Gegebenes lineares Gleichungssystem

$$
\begin{cases}
4x - 2y + 2z = 2 \\
-2x + 3y - 2z = 0 \\
3x - 5y + z = -7
\end{cases}
$$

Wir wandeln das System zunächst in eine **erweiterte Koeffizientenmatrix** um:

$$
\left[
\begin{array}{ccc|c}
4 & -2 & 2 & 2 \\
-2 & 3 & -2 & 0 \\
3 & -5 & 1 & -7
\end{array}
\right]
$$

Ziel: Die Matrix in **obere Dreiecksform** bringen.

## ✅ Schritt 1: Erste Zeile normieren (optional)

Wir lassen die erste Zeile unverändert und eliminieren stattdessen die $x$-Terme darunter.

## ✅ Schritt 2: $x$ in Zeile 2 eliminieren

Aktuelle Zeilen 1 und 2:

$$
\left[
\begin{array}{ccc|c}
4 & -2 & 2 & 2 \\
-2 & 3 & -2 & 0
\end{array}
\right]
$$

Wir wollen unter dem ersten Wert Null erzeugen. Dazu rechnen wir:

$Z_2 := Z_2 + \frac{1}{2} Z_1$

Begründung:

$-2 + \frac{1}{2}\cdot 4 = 0$

Rechnung von $Z_2$:

| Position | Rechnung     | Ergebnis |
| -------- |--------------|----------|
| 1        | $-2 + 2$     | $0$      |
| 2        | $3 + (-1)$   | $2$      |
| 3        | $-2 + 1$     | $-1$     |
|          | $0 + 1$$     | $1$$     |

→ Neue Zeile 2:

$$
\left[
\begin{array}{ccc|c}
0 & 2 & -1 & 1 
\end{array}
\right]
$$

## ✅ Schritt 3: $x$ in Zeile 3 eliminieren

Wir rechnen:

$Z_3 := Z_3 - \frac{3}{4} Z_1$

Begründung:

$3 - \frac{3}{4}\cdot 4 = 0$

Rechnung von $Z_3$:

| Position | Rechnung                   | Ergebnis          |
| -------- |----------------------------|-------------------|
| 1        | $3 - 3 = 0$                | $0$               |
| 2        | $-5 - \frac{3}{4}(-2)$     | $-5 + 1.5 = -3.5$ |
| 3        | $1 - \frac{3}{4}(2)$       | $1 - 1.5 = -0.5$  |
|          | $-7 - \frac{3}{4} \cdot 2$ | $-7 - 1.5 = -8.5$ |

→ Neue Zeile 3:

$$
\left[
\begin{array}{ccc|c}
0 & -3.5 & -0.5 & -8.5
\end{array}
\right]
$$

### Aktuelle Matrix

$$
\left[
\begin{array}{ccc|c}
4 & -2 & 2 & 2 \\
0 & 2 & -1 & 1 \\
0 & -3.5 & -0.5 & -8.5
\end{array}
\right]
$$

## ✅ Schritt 4: Zweite Zeile normieren

Wir teilen $Z_2$ durch 2:

$Z_2 := \frac{1}{2}Z_2$

neue Zeile 2:

$$
\left[
\begin{array}{ccc|c}
0 & 1 & -0.5 & 0.5
\end{array}
\right]
$$

## ✅ Schritt 5: $y$ in Zeile 3 eliminieren

Aktuell:

$$
\left[
\begin{array}{ccc|c}
0 & -3.5 & -0.5 & -8.5
\end{array}
\right]
$$

Wir rechnen:

$Z_3 := Z_3 + 3.5 Z_2$

Rechnung:

| Position | Rechnung             | Ergebnis              |
| -------- |----------------------|-----------------------|
| 1        | $0 + 3.5\cdot 0 = 0$ | $0$                   |
| 2        | $-3.5 + 3.5 = 0$     | $0$                   |
| 3        | $-0.5 + 3.5(-0.5)$   | $-0.5 - 1.75 = -2.25$ |
|          | $-8.5 + 3.5(0.5)$    | $-8.5 + 1.75 = -6.75$ |

Neue Zeile 3:

$$
\left[
\begin{array}{ccc|c}
0 & 0 & -2.25 & -6.75
\end{array}
\right]
$$

### Aktuelle Matrix:

$$
\left[
\begin{array}{ccc|c}
4 & -2 & 2 & 2 \\
0 & 1 & -0.5 & 0.5 \\
0 & 0 & -2.25 & -6.75
\end{array}
\right]
$$

## ✅ Schritt 6: Nach z auflösen

$-2.25z = -6.75$

$z = \frac{-6.75}{-2.25} = 3$

## ✅ Schritt 7: $z=3$ in Zeile 2 einsetzen

Zeile 2:

$y - 0.5z = 0.5$

Einsetzen:

$y - 0.5(3) = 0.5$

$y - 1.5 = 0.5$

$y = 2$

## ✅ Schritt 8: $y=2, z=3$ in Zeile 1 einsetzen

$4x - 2y + 2z = 2$

Einsetzen:

$4x - 4 + 6 = 2$

$4x + 2 = 2$

$4x = 0$

$x = 0$

## 🎉 Endergebnis

$$
\boxed{x = 0,\quad y = 2,\quad z = 3}
$$

