# Buch Seite 19 Aufgabe 2c: LGS mit Gauß-Verfahren lösen

$$
\begin{cases}
2x + 2y - 3z = -7 \\
-x - 2y - 2z = 3 \\
4x + y - 2z = -1
\end{cases}
$$

# 1. Erweiterte Matrix aufstellen

$$
\left[
\begin{array}{ccc|c}
2 & 2 & -3 & -7 \\
-1 & -2 & -2 & 3 \\
4 & 1 & -2 & -1
\end{array}
\right]
$$

# 2. Erste Zeile normieren

Teilen durch 2:

$Z_1 := \tfrac12 Z_1$

$$
\left[
\begin{array}{ccc|c}
1 & 1 & -1.5 & -3.5
\end{array}
\right]
$$

# 3. x unterhalb eliminieren

### $Z_2 := Z_2 + Z_1$

$$
\left[
\begin{array}{ccc|c}
0 & -1 & -3.5 & -0.5
\end{array}
\right]
$$

### $Z_3 := Z_3 - 4Z_1$

$$
\left[
\begin{array}{ccc|c}
0 & -3 & 4 & 13
\end{array}
\right]
$$

Neue Matrix:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & -1.5 & -3.5 \\
0 & -1 & -3.5 & -0.5 \\
0 & -3 & 4 & 13
\end{array}
\right]
$$

# 4. y unterhalb eliminieren

### $Z_3 := Z_3 - 3Z_2$

$$
\left[
\begin{array}{ccc|c}
0 & 0 & 4 - 3(-3.5) & 13 - 3(-0.5)
\end{array}
\right]
$$

$$
\left[
\begin{array}{ccc|c}
0 & 0 & 14.5 & 14.5
\end{array}
\right]
$$

Neue Matrix:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & -1.5 & -3.5 \\
0 & -1 & -3.5 & -0.5 \\
0 & 0 & 14.5 & 14.5
\end{array}
\right]
$$

# 5. Rückwärtseinsetzen

### Aus Zeile 3:

$14.5z = 14.5 \quad\Rightarrow\quad z = 1$

### Zeile 2:

$-y - 3.5z = -0.5$

$-y - 3.5 = -0.5$

$-y = 3$

$y = -3$

### Zeile 1:

$x + y - 1.5z = -3.5$

$x - 3 - 1.5 = -3.5$

$x - 4.5 = -3.5$

$x = 1$

# ✅ Lösung

$$
\boxed{x = 1,\quad y = -3,\quad z = 1}
$$

