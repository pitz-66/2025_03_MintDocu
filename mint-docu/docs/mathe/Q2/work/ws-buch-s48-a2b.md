# Buch Seite 48 Aufgabe 2b

Hier ist die vollständige Lösung des Gleichungssystems **mit dem Gaußschen Eliminationsverfahren** und der **Lösungsmenge**.

***

# 🔢 **Gegebenes Gleichungssystem**

$$
\begin{cases}
2x + 3y + 2z = 3 \\
4x + 5y - 2z = 1 \\
4x + 4y - 8z = -4
\end{cases}
$$

***

# ➤ **1. Erweiterte Matrix**

$$
\left(
\begin{array}{ccc|c}
2 & 3 & 2 & 3 \\
4 & 5 & -2 & 1 \\
4 & 4 & -8 & -4
\end{array}
\right)
$$

***

# ➤ **2. Eliminieren von $$x$$**

### **Z2 := Z2 − 2·Z1**

$$
(4,5,-2|1) - (4,6,4|6) = (0, -1, -6, -5)
$$

### **Z3 := Z3 − 2·Z1**

$$
(4,4,-8|-4) - (4,6,4|6) = (0, -2, -12, -10)
$$

Neue Matrix:

$$
\left(
\begin{array}{ccc|c}
2 & 3 & 2 & 3 \\
0 & -1 & -6 & -5 \\
0 & -2 & -12 & -10
\end{array}
\right)
$$

***

# ➤ **3. Eliminieren von $$y$$**

### **Z3 := Z3 − 2·Z2**

$$
(0,-2,-12|-10) - (0,-2,-12|-10) = (0,0,0,0)
$$

Zeile 3 ist überflüssig → **System hat unendlich viele Lösungen**.

***

# ➤ **4. Normieren von Zeile 2**

$$
Z_2 := -Z_2 = (0,1,6,5)
$$

Also:

$$
y + 6z = 5
\quad\Rightarrow\quad y = 5 - 6z
$$

***

# ➤ **5. Einsetzen in Zeile 1**

Zeile 1:

$$
2x + 3y + 2z = 3
$$

Setze $$y = 5 - 6z$$:

$$
2x + 3(5 - 6z) + 2z = 3
$$

$$
2x + 15 - 18z + 2z = 3
$$

$$
2x - 16z = -12
$$

$$
x - 8z = -6
$$

$$
x = -6 + 8z
$$

***

# ➤ **6. Parameterwahl**

Setze:

$$
z = t
$$

Dann:

$$
\begin{aligned}
x &= -6 + 8t \\
y &= 5 - 6t \\
z &= t
\end{aligned}
$$

***

# 🎉 **Lösungsmenge**

$$
\boxed{
L = \left\{\,(-6 + 8t,\ 5 - 6t,\ t)\ \middle|\ t \in \mathbb{R}\right\}
}
$$

Das System besitzt **unendlich viele Lösungen** (eine freie Variable $$z$$).

