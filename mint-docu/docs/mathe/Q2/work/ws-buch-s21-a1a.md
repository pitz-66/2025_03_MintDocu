# Buch Seite 21 Übung 1a: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

## 🔢 Gegebenes Gleichungssystem

$$
\begin{cases}
2x+2y+2z = 6 \\
2x + y - z = 2 \\
4x + 3y + z = 8
\end{cases}
$$

Wir verwenden das **Gauß‑Verfahren**, um zu prüfen, ob Widersprüche entstehen.

## ✅ 1. Erweiterte Matrix aufstellen

$$
\left[
\begin{array}{ccc|c}
2 & 2 & 2 & 6 \\
2 & 1 & -1 & 2 \\
4 & 3 & 1 & 8
\end{array}
\right]
$$

## ✅ 2. Erste Zeile normieren

### $Z_1 := \tfrac{1}{2}Z_1$

$$
Z_1=\left[\begin{array}{ccc|c}
1 & 1 & 1 & 3
\end{array}\right]
$$


## ✅ 3. x in Zeile 2 und 3 eliminieren

### $Z_2 := Z_2 - 2Z_1$

$$
Z_2=\left[\begin{array}{ccc|c}
0 & -1 & -3 & -4
\end{array}\right]
$$

### $Z_3 := Z_3 - 4Z_1$

$$
Z_3=\left[\begin{array}{ccc|c}
0 & -1 & -3 & -4
\end{array}\right]
$$

Neue Matrix:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 3 \\
0 & -1 & -3 & -4 \\
0 & -1 & -3 & -4
\end{array}
\right]
$$


## ✅ 4. y in Zeile 3 eliminieren

### $Z_3 := Z_3 - Z_2$

$$
Z_3=\left[\begin{array}{ccc|c}
0 & 0 & 0 & 0
\end{array}\right]
$$

Eine **Nullzeile** bedeutet:  
➡️ Das System ist **nicht widersprüchlich**.  
➡️ Es gibt **unendlich viele Lösungen**.

Der Rang der Matrix ist **2**, aber wir haben **3 Variablen** → eine **freie Variable**.

## ✅ 5. Rückwärtseinsetzen

Wir verwenden die verbliebenen beiden Zeilen:

### Zweite Zeile:

$-y - 3z = -4$

$y = -3z + 4$

### Erste Zeile:

$x + y + z = 3$

$x = 3 - y - z$

Jetzt $y$ einsetzen:

$x = 3 - ( -3z + 4 ) - z$

$x = 3 + 3z - 4 - z = -1 + 2z$

## 🎉 Lösungsmenge

Wir nehmen $z$ als freien Parameter $t$:

$$
\boxed{
\begin{aligned}
x &= -1 + 2t \\
y &= 4 - 3t \\
z &= t
\end{aligned}}
\qquad t \in \mathbb{R}
$$

In Mengenform:

$$
\boxed{
L = \{\,(-1 + 2t,\; 4 - 3t,\; t)\;|\; t \in \mathbb{R}\,\}
}
$$

## ✔️ Ergebnis

Das Gleichungssystem ist **lösbar**, nicht widersprüchlich und besitzt **unendlich viele Lösungen**.

Wenn du möchtest, kann ich die Lösung auch geometrisch (Familie von Geraden) erklären!
