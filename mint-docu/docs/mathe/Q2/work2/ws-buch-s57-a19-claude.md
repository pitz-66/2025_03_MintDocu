# Seite 57, Aufgabe 19, Rechtwinklige Dreiecke

```
Untersuche ob die Dreiecke
a) A(1|1|2), B(3|1|0), C(2|2|3)
b) A(6|2|8), B(2|6|8), C(3|6|3)
rechtwinklig sind.
```

## Lösung: Rechtwinkligkeit von Dreiecken

Ein Dreieck ist rechtwinklig, wenn zwei Seiten **senkrecht** aufeinander stehen, d.h. ihr **Skalarprodukt = 0** ist.

---

### a) A(1|1|2), B(3|1|0), C(2|2|3)

**Seitenvektoren berechnen:**

$$\vec{AB} = \begin{pmatrix}3-1\\1-1\\0-2\end{pmatrix} = \begin{pmatrix}2\\0\\-2\end{pmatrix}, \quad \vec{AC} = \begin{pmatrix}2-1\\2-1\\3-2\end{pmatrix} = \begin{pmatrix}1\\1\\1\end{pmatrix}, \quad \vec{BC} = \begin{pmatrix}2-3\\2-1\\3-0\end{pmatrix} = \begin{pmatrix}-1\\1\\3\end{pmatrix}$$

**Skalarprodukte prüfen:**

$$\vec{AB} \cdot \vec{AC} = 2\cdot1 + 0\cdot1 + (-2)\cdot1 = 2 + 0 - 2 = \mathbf{0} ✓$$

Da das Skalarprodukt **null** ist, stehen $\vec{AB}$ und $\vec{AC}$ senkrecht aufeinander.

$$\boxed{\text{Dreieck } a) \text{ ist rechtwinklig bei } A}$$

---

### b) A(6|2|8), B(2|6|8), C(3|6|3)

**Seitenvektoren berechnen:**

$$\vec{AB} = \begin{pmatrix}2-6\\6-2\\8-8\end{pmatrix} = \begin{pmatrix}-4\\4\\0\end{pmatrix}, \quad \vec{AC} = \begin{pmatrix}3-6\\6-2\\3-8\end{pmatrix} = \begin{pmatrix}-3\\4\\-5\end{pmatrix}, \quad \vec{BC} = \begin{pmatrix}3-2\\6-6\\3-8\end{pmatrix} = \begin{pmatrix}1\\0\\-5\end{pmatrix}$$

**Skalarprodukte prüfen:**

$$\vec{AB} \cdot \vec{AC} = (-4)(-3) + (4)(4) + (0)(-5) = 12 + 16 + 0 = 28 \neq 0$$

$$\vec{AB} \cdot \vec{BC} = (-4)(1) + (4)(0) + (0)(-5) = -4 + 0 + 0 = -4 \neq 0$$

$$\vec{AC} \cdot \vec{BC} = (-3)(1) + (4)(0) + (-5)(-5) = -3 + 0 + 25 = 22 \neq 0$$

Kein Skalarprodukt ist null.

$$\boxed{\text{Dreieck } b) \text{ ist } \textbf{nicht} \text{ rechtwinklig}}$$