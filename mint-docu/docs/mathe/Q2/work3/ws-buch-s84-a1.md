## Übung 1 – Winkel zwischen Vektoren

**Aufgabe:** Bestimmen Sie den Winkel zwischen den Vektoren $\vec{a}$ und $\vec{b}$ mithilfe der Formel:

$$\cos(\varphi) = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| \cdot |\vec{b}|}$$

---

### a) $\vec{a} = \begin{pmatrix}3\\1\end{pmatrix}, \quad \vec{b} = \begin{pmatrix}3\\-3\end{pmatrix}$

**Skalarprodukt:**
$$\vec{a} \cdot \vec{b} = 3\cdot3 + 1\cdot(-3) = 9 - 3 = 6$$

**Beträge:**
$$|\vec{a}| = \sqrt{3^2+1^2} = \sqrt{10}, \qquad |\vec{b}| = \sqrt{3^2+(-3)^2} = \sqrt{18}$$

**Winkel:**
$$\cos(\varphi) = \frac{6}{\sqrt{10}\cdot\sqrt{18}} = \frac{6}{\sqrt{180}} = \frac{6}{6\sqrt{5}} = \frac{1}{\sqrt{5}}$$

$$\boxed{\varphi = \arccos\!\left(\tfrac{1}{\sqrt{5}}\right) \approx 63{,}43°}$$

---

### b) $\vec{a} = \begin{pmatrix}1\\2\\-3\end{pmatrix}, \quad \vec{b} = \begin{pmatrix}-2\\-4\\0\end{pmatrix}$

**Skalarprodukt:**
$$\vec{a} \cdot \vec{b} = 1\cdot(-2) + 2\cdot(-4) + (-3)\cdot0 = -2 - 8 + 0 = -10$$

**Beträge:**
$$|\vec{a}| = \sqrt{1+4+9} = \sqrt{14}, \qquad |\vec{b}| = \sqrt{4+16+0} = \sqrt{20}$$

**Winkel:**
$$\cos(\varphi) = \frac{-10}{\sqrt{14}\cdot\sqrt{20}} = \frac{-10}{\sqrt{280}} = \frac{-10}{2\sqrt{70}}= \frac{-5}{\sqrt{70}}$$

$$\boxed{\varphi = \arccos\!\left(\tfrac{-5}{\sqrt{70}}\right) \approx 126{,}87°}$$

---

### c) $\vec{a} = \begin{pmatrix}4\\3\\4\end{pmatrix}, \quad \vec{b} = \begin{pmatrix}2\\-4\\1\end{pmatrix}$

**Skalarprodukt:**
$$\vec{a} \cdot \vec{b} = 4\cdot2 + 3\cdot(-4) + 4\cdot1 = 8 - 12 + 4 = 0$$

Da das Skalarprodukt **null** ist:

$$\boxed{\varphi = 90° \quad \text{(die Vektoren sind senkrecht zueinander)}}$$