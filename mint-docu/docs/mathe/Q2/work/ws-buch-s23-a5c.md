# Buch Seite 23, Aufgabe 5c: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

# 🔢 **Gegebenes Gleichungssystem**

$$
\begin{cases}
x_1 + x_3 = x_2 \\
x_2 + x_5 = x_4 \\
x_5 - x_3 = 0 \\
x_4 - x_2 = x_3 \\
x_4 - x_1 = x_3 + x_5
\end{cases}
$$

Wir bringen alle Gleichungen in die Form „linke Seite – rechte Seite = 0“.

***

# ➤ **1. Umformen in Standardform**

1.  $$x_1 + x_3 - x_2 = 0$$
2.  $$x_2 + x_5 - x_4 = 0$$
3.  $$-x_3 + x_5 = 0$$
4.  $$-x_2 + x_3 + x_4 = 0$$
5.  $$-x_1 + x_3 + x_5 + x_4 = 0$$

***

# ➤ **2. Erweiterte Matrix**

Variablen in der Reihenfolge:  
$$(x_1, x_2, x_3, x_4, x_5)$$

$$
\left(
\begin{array}{ccccc|c}
1 & -1 & 1 & 0 & 0 & 0 \\
0 & 1 & 0 & -1 & 1 & 0 \\
0 & 0 & -1 & 0 & 1 & 0 \\
0 & -1 & 1 & 1 & 0 & 0 \\
-1 & 0 & 1 & 1 & 1 & 0
\end{array}
\right)
$$

***

# ➤ **3. Gauß-Elimination**

### (a) Nutze Zeile 1 als Pivot, eliminiere $$x_1$$ aus Zeile 5:

$$
Z_5 \leftarrow Z_5 + Z_1
$$

Ergebnis:

$$
(0,\ -1,\ 2,\ 1,\ 1\ |\ 0)
$$

***

### (b) Nun Zeile 2 als Pivot für $$x_2$$

Eliminiere $$x_2$$ aus Zeile 4 und Zeile 5:

$$
Z_4 \leftarrow Z_4 + Z_2,\quad Z_5 \leftarrow Z_5 + Z_2
$$

Ergebnisse:

$$
Z_4 = (0, 0, 1, 0, 1\ |\ 0)
$$

$$
Z_5 = (0, 0, 2, 0, 2\ |\ 0)
$$

***

### (c) Pivot $$x_3$$ in Zeile 3

Zeile 3 lautet:

$$
(0,0,-1,0,1|0)
$$

Zeile 4 lautet:

$$
(0,0,1,0,1|0)
$$

Zeile 5 ist proportional zu Zeile 4 → remove redundant equation.

Multiplikation von Zeile 3 mit $$-1$$:

$$
Z_3 = (0,0,1,0,-1|0)
$$

***

### (d) Vergleiche Zeile 3 und Zeile 4:

$$
Z_4 - Z_3 = (0,0,0,0,2|0)
$$

→ Das bedeutet:

$$
2x_5 = 0 \quad\Rightarrow\quad x_5 = 0
$$

***

# ➤ **4. Rückwärtseinsetzen**

### Aus $$x_5 = 0$$:

Aus Zeile 3:

$$
x_3 - x_5 = 0 \Rightarrow x_3 = 0
$$

Aus Zeile 2:

$$
x_2 - x_4 + x_5 = 0 \Rightarrow x_2 = x_4
$$

Aus Zeile 1:

$$
x_1 + x_3 - x_2 = 0
$$

$$
x_1 = x_2
$$

***

# ➤ **5. Zusammenfassung**

Wir haben:

$$
x_5 = 0,\quad x_3 = 0,\quad x_2 = x_4,\quad x_1 = x_2
$$

Setze Parameter:

$$
x_2 = s
$$

$$
x_4 = s,\quad x_1 = s
$$

Damit:

$$
(x_1, x_2, x_3, x_4, x_5) = (s, s, 0, s, 0)
$$

***

# 🎉 **Lösungsmenge**

$$
\boxed{
L = \left\{ (s,\, s,\, 0,\, s,\, 0)\ \middle|\ s \in \mathbb{R} \right\}
}
$$

Das System hat also **eine freie Variable** und **unendlich viele Lösungen**, die entlang einer Geraden im $$\mathbb{R}^5$$ liegen.


