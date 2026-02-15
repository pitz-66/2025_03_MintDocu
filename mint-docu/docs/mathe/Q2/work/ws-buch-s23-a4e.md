# Buch Seite 23, Aufgabe 4e: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

# 🔢 Gegebenes Gleichungssystem

$$
\begin{cases}
3x - y + 2z = 4 \\
4x - 6y + 4z = 10 \\
-x - 2y = 1
\end{cases}
$$

***

# ➤ **1. Aufstellen der erweiterten Matrix**

$$
\left(
\begin{array}{ccc|c}
3 & -1 & 2 & 4 \\
4 & -6 & 4 & 10 \\
-1 & -2 & 0 & 1
\end{array}
\right)
$$

***

# ➤ **2. Pivot in Zeile 1 erzeugen**

Wir nutzen Zeile 1 als Pivot.

***

# ➤ **3. $$x$$ aus Zeile 2 eliminieren**

Operation:

$$
Z_2 \leftarrow Z_2 - \frac{4}{3} Z_1
$$

Berechnung:

*   $$4 - 4 = 0$$
*   $$-6 - \left(-\frac{4}{3}\right) = -6 + \frac{4}{3} = -\frac{14}{3}$$
*   $$4 - \frac{8}{3} = \frac{4}{3}$$
*   $$10 - \frac{16}{3} = \frac{14}{3}$$

Neue Zeile 2:

$$
\left( 0, -\frac{14}{3}, \frac{4}{3}, \frac{14}{3} \right)
$$

***

# ➤ **4. $$x$$ aus Zeile 3 eliminieren**

Operation:

$$
Z_3 \leftarrow Z_3 + \frac{1}{3} Z_1
$$

Berechnung:

*   $$-1 + 1 = 0$$
*   $$-2 + \left(-\frac{1}{3}\right) = -\frac{7}{3}$$
*   $$0 + \frac{2}{3} = \frac{2}{3}$$
*   $$1 + \frac{4}{3} = \frac{7}{3}$$

Neue Zeile 3:

$$
\left( 0, -\frac{7}{3}, \frac{2}{3}, \frac{7}{3} \right)
$$

***

# ➤ **5. Jetzt vergleichen wir Zeile 2 und Zeile 3**

Zeile 2:

$$
0,\ -\frac{14}{3},\ \frac{4}{3},\ \frac{14}{3}
$$

Zeile 3:

$$
0,\ -\frac{7}{3},\ \frac{2}{3},\ \frac{7}{3}
$$

Man sieht:

$$
Z_2 = 2 \cdot Z_3
$$

→ **Zeilen sind proportional**, also **keine neue Information**.

Das System ist **nicht widersprüchlich**, aber es hat **unendlich viele Lösungen**.

Wir haben ein **unterbestimmtes System** → **ein Parameter**.

***

# ➤ **6. Weiter vereinfachen**

Reduziere Zeile 3 durch Multiplikation mit $$-3/7$$:

$$
Z_3 \leftarrow -\frac{3}{7} Z_3
$$

Dann wird:

$$
(0, 1, -\tfrac{2}{7}, -1)
$$

***

# ➤ **7. Backward‑Einsetzen**

Wir haben nun:

$$
\begin{aligned}
3x - y + 2z &= 4 \\
y - \frac{2}{7} z &= -1
\end{aligned}
$$

Löse nach $$y$$:

$$
y = -1 + \frac{2}{7}z
$$

Setze in Gleichung 1 ein:

$$
3x - \left(-1 + \frac{2}{7}z\right) + 2z = 4
$$

$$
3x + 1 - \frac{2}{7}z + 2z = 4
$$

$$
3x + 1 + \frac{12}{7}z = 4
$$

$$
3x = 3 - \frac{12}{7}z
$$

$$
x = 1 - \frac{4}{7}z
$$

***

# ✅ **8. Parameterform (mit $$z = t$$)**

Setze $$z = t$$:

$$
\begin{aligned}
x &= 1 - \frac{4}{7} t \\
y &= -1 + \frac{2}{7} t \\
z &= t
\end{aligned}
$$

***

# 🎉 **Lösungsmenge**

$$
\boxed{
L = \left\{ 
\left(1 - \frac{4}{7}t,\ -1 + \frac{2}{7}t,\ t\right)
\;\middle|\; t \in \mathbb{R}
\right\}
}
$$

Das System besitzt also **unendlich viele Lösungen**, die sich entlang einer Geraden im $$\mathbb{R}^3$$ erstrecken.


