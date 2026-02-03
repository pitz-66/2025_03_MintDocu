# Buch Seite 19 Aufgabe 2b: LGS mit Gauß-Verfahren lösen

$$
\begin{cases}
x + 2y - 2z = -4 \\
2x + y + z = 3 \\
3x + 2y + z = 4
\end{cases}
$$

## 1. Erweiterte Matrix aufstellen

$$
\left[
\begin{array}{ccc|c}
1 & 2 & -2 & -4 \\
2 & 1 & 1 & 3 \\
3 & 2 & 1 & 4
\end{array}
\right]
$$

## 2. Unter dem ersten x Nullen erzeugen

### $Z_2 := Z_2 - 2Z_1$

Ergebnis:

$$
\left[
\begin{array}{ccc|c}
0 & -3 & 5 & 11 
\end{array}
\right]
$$

### $Z_3 := Z_3 - 3Z_1$

Ergebnis:

$$
\left[
\begin{array}{ccc|c}
0 & -4 & 7 & 16 
\end{array}
\right]
$$

Matrix:

$$
\left[
\begin{array}{ccc|c}
1 & 2 & -2 & -4 \\
0 & -3 & 5 & 11 \\
0 & -4 & 7 & 16
\end{array}
\right]
$$

## 3. Unter dem zweiten y Null erzeugen

Normieren von $Z_2$ ist nicht nötig.

### $Z_3 := Z_3 - \frac{4}{3} Z_2$

Ergebnis:

$$
\left[
\begin{array}{ccc|c}
0 & 0 & \frac{1}{3} & \frac{4}{3}
\end{array}
\right]
$$

Matrix:

$$
\left[
\begin{array}{ccc|c}
1 & 2 & -2 & -4 \\
0 & -3 & 5 & 11 \\
0 & 0 & \frac{1}{3} & \frac{4}{3}
\end{array}
\right]
$$

## 4. Rückwärtseinsetzen

### Aus Zeile 3:

$\frac13 z = \frac43 \quad\Rightarrow\quad z = 4$

### In Zeile 2:

$-3y + 5z = 11$

$-3y + 20 = 11$

$y = 3$

### In Zeile 1:

$x + 2\cdot 3 - 2\cdot 4 = -4$

$x + 6 - 8 = -4$

$x = -2$

## ✅ Lösung

$$
\boxed{x = -2,\quad y = 3,\quad z = 4}
$$

