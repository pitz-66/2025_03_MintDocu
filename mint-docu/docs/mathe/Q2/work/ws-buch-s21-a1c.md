# Buch Seite 21 Übung 1c: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

## 🔢 Gegebenes lineares Gleichungssystem

$$
\begin{cases}
4x - 3y - 5z = 9 \\
2x + 5y - 9z = 11 \\
6x - 11y - z = 7
\end{cases}
$$

Wir nutzen den **Gauß‑Algorithmus**.

## ✅ 1. Erweiterte Matrix

$$
\left[
\begin{array}{ccc|c}
4 & -3 & -5 & 9 \\
2 & 5 & -9 & 11 \\
6 & -11 & -1 & 7
\end{array}
\right]
$$

## ✅ 2. Erste Spalte unter Zeile 1 eliminieren

### $Z_2 := Z_2 - \tfrac{1}{2} Z_1$

$(2,\; 5,\; -9,\; 11) - (2,\; -1.5,\; -2.5,\; 4.5)$

$Z_2 = (0,\; 6.5,\; -6.5,\; 6.5)$

### $Z_3 := Z_3 - \tfrac{3}{2} Z_1$

$(6,\; -11,\; -1,\; 7) - (6,\; -4.5,\; -7.5,\; 13.5)$

$Z_3 = (0,\; -6.5,\; 6.5,\; -6.5)$

Neue Matrix:

$$
\left[
\begin{array}{ccc|c}
4 & -3 & -5 & 9 \\
0 & 6.5 & -6.5 & 6.5 \\
0 & -6.5 & 6.5 & -6.5
\end{array}
\right]
$$

## ✅ 3. Zweite Spalte unter Zeile 2 eliminieren

### $Z_3 := Z_3 + Z_2$

$(0,\; -6.5,\; 6.5,\; -6.5) + (0,\; 6.5,\; -6.5,\; 6.5)$

$Z_3 = (0,\; 0,\; 0,\; 0)$

Wir erhalten eine **Nullzeile**, aber **keine widersprüchliche Zeile** →  
➡️ Das System hat **unendlich viele Lösungen**.

## ✅ 4. Rückwärtseinsetzen

Zweite Zeile (durch 6,5 teilen):

$y - z = 1$

$y = z + 1$

Erste Zeile:

$4x - 3y - 5z = 9$

Einsetzen von $y$:

$4x - 3(z+1) - 5z = 9$

$4x - 3z - 3 - 5z = 9$

$4x - 8z = 12$

$x = 3 + 2z$

## 🔷 5. Lösungsmenge

Wir wählen $z = t$ als freien Parameter.

$$
\boxed{
\begin{aligned}
x &= 3 + 2t \\
y &= 1 + t \\
z &= t
\end{aligned}}
\qquad t \in \mathbb{R}
$$

In Mengenform:

$$
\boxed{
L = \{\, (3 + 2t,\; 1 + t,\; t) \mid t \in \mathbb{R} \,\}
}
$$

## 🎉 Ergebnis

Das Gleichungssystem ist **lösbar**, aber nicht eindeutig:

$$
\textbf{Es besitzt unendlich viele Lösungen.}
$$
