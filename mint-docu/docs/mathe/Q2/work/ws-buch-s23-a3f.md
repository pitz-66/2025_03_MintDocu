# Buch Seite 23 Aufgabe 3f

# 🔢 **Gegebenes Gleichungssystem**

$$
\begin{cases}
x + y + z = 5 \\
x - y + z = 1 \\
-2x - 3z = -3
\end{cases}
$$

***

# ➤ **1. Erweiterte Matrix**

$$
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 5 \\
1 & -1 & 1 & 1 \\
-2 & 0 & -3 & -3
\end{array}
\right)
$$

***

# ➤ **2. Eliminieren von $$x$$**

### **Z2 := Z2 − Z1**

$$
(1,-1,1|1) - (1,1,1|5) = (0,-2,0|-4)
$$

### **Z3 := Z3 + 2·Z1**

$$
(-2,0,-3|-3) + (2,2,2|10) = (0,2,-1|7)
$$

Neue Matrix:

$$
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 5 \\
0 & -2 & 0 & -4 \\
0 & 2 & -1 & 7
\end{array}
\right)
$$

***

# ➤ **3. Normieren der zweiten Zeile**

### **Z2 := Z2 / (-2)**

$$
(0,1,0|2)
$$

***

# ➤ **4. Eliminieren von $$y$$**

### **Z3 := Z3 − 2·Z2**

$$
(0,2,-1|7) - (0,2,0|4) = (0,0,-1|3)
$$

***

# ➤ **5. Normieren von Zeile 3**

### **Z3 := −Z3**

$$
(0,0,1|-3)
$$

Damit:

$$
z = -3
$$

***

# ➤ **6. Rückwärtseinsetzen**

### **Aus Zeile 2:**

$$
y = 2
$$

### **Aus Zeile 1:**

$$
x + y + z = 5
$$

$$
x + 2 + (-3) = 5
$$

$$
x - 1 = 5 \quad\Rightarrow\quad x = 6
$$

***

# 🎉 **Lösung**

$$
\boxed{x = 6,\quad y = 2,\quad z = -3}
$$

***

# ✅ **Lösungsmenge**

$$
\boxed{
L = \{(6,\ 2,\ -3)\}
}
$$

Das Gleichungssystem besitzt **eine eindeutige Lösung**.

