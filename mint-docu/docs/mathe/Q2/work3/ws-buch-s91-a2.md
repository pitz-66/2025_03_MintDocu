## Aufgabe 2 – Betrag eines Vektors

**Gegeben:**
$$\vec{a} = \begin{pmatrix}1\\4\\8\end{pmatrix}, \quad \vec{b} = \begin{pmatrix}4\\4\\7\end{pmatrix}, \quad \vec{c} = \begin{pmatrix}2\\6\\9\end{pmatrix}, \quad \overrightarrow{AB} = \begin{pmatrix}2\\x\\11\end{pmatrix}$$

- **a)** Untersuchen Sie, welcher der Vektoren $\vec{a}$ oder $\vec{b}$ den längeren Pfeil hat.
- **b)** Bestimmen Sie die fehlende Koordinate $x$ so, dass der Pfeil $\overrightarrow{AB}$ die Länge **15** hat.

---

## Teil a) Vergleich der Beträge von $\vec{a}$ und $\vec{b}$

Die Länge (Betrag) eines Vektors berechnet sich mit:
$$|\vec{v}| = \sqrt{v_1^2 + v_2^2 + v_3^2}$$

**Betrag von $\vec{a}$:**
$$|\vec{a}| = \sqrt{1^2 + 4^2 + 8^2} = \sqrt{1 + 16 + 64} = \sqrt{81} = 9$$

**Betrag von $\vec{b}$:**
$$|\vec{b}| = \sqrt{4^2 + 4^2 + 7^2} = \sqrt{16 + 16 + 49} = \sqrt{81} = 9$$

$$\boxed{|\vec{a}| = |\vec{b}| = 9}$$

> Beide Vektoren haben **dieselbe Länge** – keiner ist länger als der andere!

---

## Teil b) Fehlende Koordinate x bestimmen

**Bedingung:** $|\overrightarrow{AB}| = 15$

$$|\overrightarrow{AB}| = \sqrt{2^2 + x^2 + 11^2} = 15$$

$$\sqrt{4 + x^2 + 121} = 15 \qquad |^2$$

$$x^2 + 125 = 225$$

$$x^2 = 100$$

$$\boxed{x = 10 \quad \text{oder} \quad x = -10}$$

**Probe:**
$$\left|\begin{pmatrix}2\\\pm10\\11\end{pmatrix}\right| = \sqrt{4 + 100 + 121} = \sqrt{225} = 15 \quad \checkmark$$