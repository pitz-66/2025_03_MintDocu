# Buch Seite 23, Aufgabe 4d: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

# 🔢 Gegebenes Gleichungssystem

$$
\begin{cases}
2x - 3y - 8z = 8 \\
6y + 4z = -8 \\
6x + 8y - 8z = 6
\end{cases}
$$

***

# ➤ **1. Aufstellen der erweiterten Matrix**

$$
\left(
\begin{array}{ccc|c}
2 & -3 & -8 & 8 \\
0 &  6 &  4 & -8 \\
6 &  8 & -8 & 6
\end{array}
\right)
$$

***

# ➤ **2. Eliminieren von $$x$$ aus Zeile 3**

Wir nutzen $$Z_1$$ als Pivotzeile.

Operation:

$$
Z_3 \leftarrow Z_3 - 3 Z_1
$$

Berechnung:

*   $$6 - 3\cdot 2 = 0$$
*   $$8 - 3(-3) = 17$$
*   $$-8 - 3(-8) = 16$$
*   $$6 - 3\cdot 8 = -18$$

Neue Matrix:

$$
\left(
\begin{array}{ccc|c}
2 & -3 & -8 & 8 \\
0 & 6 & 4 & -8 \\
0 & 17 & 16 & -18
\end{array}
\right)
$$

***

# ➤ **3. Zweite Pivotzeile normieren**

$$
Z_2 \leftarrow \frac{1}{6} Z_2
$$

$$
\left(
\begin{array}{ccc|c}
2 & -3 & -8 & 8 \\
0 & 1 & \frac{2}{3} & -\frac{4}{3} \\
0 & 17 & 16 & -18
\end{array}
\right)
$$

***

# ➤ **4. Eliminieren des $$y$$ in Zeile 3**

Operation:

$$
Z_3 \leftarrow Z_3 - 17 Z_2
$$

Berechnung:

*   $$17 - 17 = 0$$
*   $$16 - 17\cdot \frac{2}{3} = 16 - \frac{34}{3} = \frac{48-34}{3}= \frac{14}{3}$$
*   $$-18 - 17\left(-\frac{4}{3}\right) = -18 + \frac{68}{3} = \frac{-54+68}{3} = \frac{14}{3}$$

Neue Zeile 3:

$$
(0,\ 0,\ \tfrac{14}{3}\ |\ \tfrac{14}{3})
$$

***

# ➤ **5. Normieren der dritten Zeile**

$$
Z_3 \leftarrow \frac{3}{14} Z_3
$$

$$
(0,\ 0,\ 1\ |\ 1)
$$

Also:

$$
z = 1
$$

***

# ➤ **6. Rückwärtseinsetzen**

## Aus Zeile 2:

$$
y + \frac{2}{3} z = -\frac{4}{3}
$$

Einsetzen von $$z=1$$:

$$
y + \frac{2}{3} = -\frac{4}{3}
$$

$$
y = -2
$$

## Aus Zeile 1:

$$
2x - 3y - 8z = 8
$$

Einsetzen von $$y=-2,\ z=1$$:

$$
2x - 3(-2) - 8 = 8
$$

$$
2x + 6 - 8 = 8
$$

$$
2x - 2 = 8
$$

$$
x = 5
$$

***

# ✅ **Lösung**

$$
\boxed{x = 5,\quad y = -2,\quad z = 1}
$$

***

# 🎉 **Lösungsmenge**

$$
\boxed{
L = \{(5,\ -2,\ 1)\}
}
$$

Das System besitzt **eine eindeutige Lösung**.


