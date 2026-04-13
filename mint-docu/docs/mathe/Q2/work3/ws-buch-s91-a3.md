## Aufgabe 3 – Dreieck

**Gegeben:** $A(1|2|3)$, $B(2|7|6)$, $C(-3|2|2)$

- **a)** Weisen Sie nach, dass $A$, $B$ und $C$ die Eckpunkte eines Dreiecks sind.
- **b)** Überprüfen Sie, ob das Dreieck $ABC$ gleichschenklig oder rechtwinklig ist.
- **c)** Ergänzen Sie $ABC$ durch Hinzunahme eines Punktes $D$ zum Parallelogramm $ABCD$.

---

## Teil a) Nachweis: A, B, C sind Eckpunkte eines Dreiecks

Drei Punkte bilden ein Dreieck, wenn sie **nicht kollinear** sind, d.h. $\vec{AB}$ und $\vec{AC}$ sind **nicht parallel**.

**Seitenvektoren berechnen:**

$$\vec{AB} = B - A = \begin{pmatrix}2-1\\7-2\\6-3\end{pmatrix} = \begin{pmatrix}1\\5\\3\end{pmatrix}$$

$$\vec{AC} = C - A = \begin{pmatrix}-3-1\\2-2\\2-3\end{pmatrix} = \begin{pmatrix}-4\\0\\-1\end{pmatrix}$$

$$\vec{BC} = C - B = \begin{pmatrix}-3-2\\2-7\\2-6\end{pmatrix} = \begin{pmatrix}-5\\-5\\-4\end{pmatrix}$$

**Kollinearitätsprüfung:** $\vec{AB} = k \cdot \vec{AC}$ würde bedeuten:

$$1 = k\cdot(-4), \quad 5 = k\cdot0, \quad 3 = k\cdot(-1)$$

Die zweite Gleichung $5 = 0$ ist ein **Widerspruch** → die Vektoren sind **nicht parallel**.

$$\boxed{A,\ B,\ C \text{ sind nicht kollinear} \Rightarrow \text{sie bilden ein Dreieck.} \checkmark}$$

---

## Teil b) Gleichschenklig oder rechtwinklig?

### Seitenlängen berechnen:

$$|AB| = \sqrt{1^2+5^2+3^2} = \sqrt{1+25+9} = \sqrt{35}$$

$$|AC| = \sqrt{(-4)^2+0^2+(-1)^2} = \sqrt{16+0+1} = \sqrt{17}$$

$$|BC| = \sqrt{(-5)^2+(-5)^2+(-4)^2} = \sqrt{25+25+16} = \sqrt{66}$$

### Gleichschenklig?

Zwei Seiten müssten gleich lang sein:

$$\sqrt{35} \neq \sqrt{17} \neq \sqrt{66}$$

$$\boxed{\text{Das Dreieck ist \textbf{nicht} gleichschenklig.}}$$

### Rechtwinklig?

Skalarprodukte aller Seitenpaare prüfen:

$$\vec{AB} \cdot \vec{AC} = (1)(-4)+(5)(0)+(3)(-1) = -4+0-3 = -7 \neq 0$$

$$\vec{AB} \cdot \vec{BC} = (1)(-5)+(5)(-5)+(3)(-4) = -5-25-12 = -42 \neq 0$$

$$\vec{AC} \cdot \vec{BC} = (-4)(-5)+(0)(-5)+(-1)(-4) = 20+0+4 = 24 \neq 0$$

$$\boxed{\text{Das Dreieck ist \textbf{nicht} rechtwinklig.}}$$

---

## Teil c) Punkt D zum Parallelogramm ABCD

Bei einem Parallelogramm $ABCD$ gilt:

$$\vec{AB} = \vec{DC} \quad \Longrightarrow \quad D = C - \vec{AB} \quad \text{bzw.} \quad D = A + \vec{AC} + \vec{AB} - \vec{AB}$$

Einfacher: Da $\overrightarrow{AB} = \overrightarrow{DC}$ gelten muss, folgt:

$$D = A + \vec{AC} = A + (C - A) \quad \text{...nein, korrekt via Mittelpunkt:}$$

Der Mittelpunkt der Diagonale $AC$ muss gleich dem Mittelpunkt der Diagonale $BD$ sein:

$$M = \frac{A + C}{2} = \frac{B + D}{2} \quad \Rightarrow \quad D = A + C - B$$

$$D = \begin{pmatrix}1\\2\\3\end{pmatrix} + \begin{pmatrix}-3\\2\\2\end{pmatrix} - \begin{pmatrix}2\\7\\6\end{pmatrix} = \begin{pmatrix}1-3-2\\2+2-7\\3+2-6\end{pmatrix}$$

$$\boxed{D = (-4\ |\ {-3}\ |\ {-1})}$$

**Probe:** $\vec{DC} = C - D = \begin{pmatrix}-3-(-4)\\2-(-3)\\2-(-1)\end{pmatrix} = \begin{pmatrix}1\\5\\3\end{pmatrix} = \vec{AB} \checkmark$