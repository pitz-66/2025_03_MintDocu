# Buch Seite 23, Aufgabe 5b: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

# 🔢 **Gegebenes Gleichungssystem**

$$
\begin{cases}
x_1 + x_3 = 1 \\
x_2 - x_3 = 0 \\
x_1 + x_2 + x_3 - x_4 = 1 \\
x_2 - x_4 = 0
\end{cases}
$$

***

# ➤ **1. Aufstellen der erweiterten Matrix**

Ordnung der Variablen: $$x_1, x_2, x_3, x_4$$

$$
\left(
\begin{array}{cccc|c}
1 & 0 & 1 & 0 & 1 \\
0 & 1 & -1 & 0 & 0 \\
1 & 1 & 1 & -1 & 1 \\
0 & 1 & 0 & -1 & 0
\end{array}
\right)
$$

***

# ➤ **2. Eliminiere $$x_1$$ aus Zeile 3**

$$
Z_3 \leftarrow Z_3 - Z_1
$$

Ergebnis:

$$
(0,\ 1,\ 0,\ -1\ |\ 0)
$$

Das ist **identisch mit Zeile 4** → Zeile 4 enthält keine neue Information.

Neue Matrix:

$$
\left(
\begin{array}{cccc|c}
1 & 0 & 1 & 0 & 1 \\
0 & 1 & -1 & 0 & 0 \\
0 & 1 & 0 & -1 & 0 \\
0 & 1 & 0 & -1 & 0
\end{array}
\right)
$$

Wir streichen Zeile 4.

***

# ➤ **3. Eliminiere $$x_2$$ aus Zeile 3**

$$
Z_3 \leftarrow Z_3 - Z_2
$$

Rechnung:

*   $$1 - 1 = 0$$
*   $$0 - (-1) = 1$$
*   $$-1 - 0 = -1$$
*   $$0 - 0 = 0$$

Ergebnis:

$$
(0,\ 0,\ 1,\ -1\ |\ 0)
$$

Neue Matrix:

$$
\left(
\begin{array}{cccc|c}
1 & 0 & 1 & 0 & 1 \\
0 & 1 & -1 & 0 & 0 \\
0 & 0 & 1 & -1 & 0 \\
\end{array}
\right)
$$

***

# ➤ **4. Rückwärtseinsetzen**

### **Aus Zeile 3:**

$$
x_3 - x_4 = 0 \quad\Rightarrow\quad x_3 = x_4
$$

### **Aus Zeile 2:**

$$
x_2 - x_3 = 0
$$

$$
x_2 = x_3 = x_4
$$

### **Aus Zeile 1:**

$$
x_1 + x_3 = 1
$$

$$
x_1 = 1 - x_3 = 1 - x_4
$$

***

# 🎉 **Lösungsmenge in Parameterform**

Wir setzen den freien Parameter $$x_4 = t$$:

$$
\begin{aligned}
x_1 &= 1 - t \\
x_2 &= t \\
x_3 &= t \\
x_4 &= t
\end{aligned}
$$

***

# ✅ **Lösungsmenge**

$$
\boxed{
L = \left\{
(1-t,\ t,\ t,\ t)\ \middle|\ t \in \mathbb{R}
\right\}
}
$$

Das System besitzt **unendlich viele Lösungen** und eine frei wählbare Variable $$x_4$$.

