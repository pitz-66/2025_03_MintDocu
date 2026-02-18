# Buch Seite 23 Aufgabe 3d

# 🔢 **Gegebenes Gleichungssystem**

$$
\begin{cases}
-2x + 2y - 4z = -2 \\
x + 3z = 0 \\
x - y + 2z = 1
\end{cases}
$$

***

# ➤ **1. Umformen und Matrix aufstellen**

$$
\left(
\begin{array}{ccc|c}
-2 & 2 & -4 & -2 \\
1 & 0 & 3 & 0 \\
1 & -1 & 2 & 1
\end{array}
\right)
$$

Wir vertauschen Zeile 1 und Zeile 2 (bessere Pivot‑Wahl):

$$
\left(
\begin{array}{ccc|c}
1 & 0 & 3 & 0 \\
-2 & 2 & -4 & -2 \\
1 & -1 & 2 & 1
\end{array}
\right)
$$

***

# ➤ **2. Eliminieren von $$x$$**

### **Z2 := Z2 + 2·Z1**

$$
(-2,2,-4|-2)+ (2,0,6|0) = (0,2,2|-2)
$$

### **Z3 := Z3 − Z1**

$$
(1,-1,2|1)-(1,0,3|0) = (0,-1,-1|1)
$$

Neue Matrix:

$$
\left(
\begin{array}{ccc|c}
1 & 0 & 3 & 0 \\
0 & 2 & 2 & -2 \\
0 & -1 & -1 & 1
\end{array}
\right)
$$

***

# ➤ **3. Eliminieren von $$y$$**

Normiere Zeile 2:

### **Z2 := ½·Z2**

$$
(0,1,1|-1)
$$

Eliminiere $$y$$ aus Zeile 3:

### **Z3 := Z3 + Z2**

$$
(0,-1,-1|1) + (0,1,1|-1) = (0,0,0|0)
$$

Zeile 3 liefert **keine neue Information** → System *unterbestimmt* → **unendlich viele Lösungen**.

Aktuelle Matrix lautet:

$$
\left(
\begin{array}{ccc|c}
1 & 0 & 3 & 0 \\
0 & 1 & 1 & -1 \\
0 & 0 & 0 & 0
\end{array}
\right)
$$

***

# ➤ **4. Rückwärtseinsetzen**

### Aus Zeile 2:

$$
y + z = -1
$$

$$
y = -1 - z
$$

### Aus Zeile 1:

$$
x + 3z = 0
$$

$$
x = -3z
$$

Setze $$z = t$$ als freien Parameter.

***

# 🎉 **Lösungsmenge**

$$
\boxed{
L = \left\{\, (-3t,\ -1 - t,\ t)\ \middle|\ t \in \mathbb{R} \right\}
}
$$

Das System besitzt **unendlich viele Lösungen**, eine **freie Variable** ($$z$$).


