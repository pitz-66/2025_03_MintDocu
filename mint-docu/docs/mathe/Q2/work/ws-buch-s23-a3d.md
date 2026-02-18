# Buch Seite 23 Aufgabe 3d

# 🔢 **Gegebenes Gleichungssystem**

$$
\begin{cases}
x + 2y - z = -3 \\
2x + 4y - 2z = -1 \\
3x + y + 5z = 6
\end{cases}
$$

***

# ➤ **1. Erweiterte Matrix**

$$
\left(
\begin{array}{ccc|c}
1 & 2 & -1 & -3 \\
2 & 4 & -2 & -1 \\
3 & 1 & 5 & 6
\end{array}
\right)
$$

***

# ➤ **2. Eliminieren von $$x$$**

### **Zeile 2:**

$$
Z_2 \leftarrow Z_2 - 2Z_1
$$

$$
(2,4,-2|-1) - (2,4,-2|-6) = (0,0,0|5)
$$

Ergebnis Zeile 2:

$$
(0,0,0|5)
$$

Das bedeutet:

$$
0 = 5
$$

Das ist **ein Widerspruch**.

### **Zeile 3:**

$$
Z_3 \leftarrow Z_3 - 3Z_1
$$

Doch das ist nicht einmal mehr nötig — bereits **eine einzige widersprüchliche Zeile** zeigt:

***

# ❗ **Widerspruch → keine Lösung**

Die Zeile

$$
(0,0,0|5)
$$

bedeutet:

$$
0 = 5
$$

Das ist **unmöglich**.

Damit ist das Gleichungssystem **inkonsistent**.

***

# ✅ **Lösungsmenge**

$$
\boxed{L = \emptyset}
$$

Das System hat **keine Lösung**.


