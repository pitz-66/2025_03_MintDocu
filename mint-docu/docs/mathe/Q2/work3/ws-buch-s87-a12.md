## Aufgabe 12 – Winkel im Quader

**Aufgabe:** Ein Quader hat die Grundflächenmaße $4 \times 3$. Wie muss die Höhe $h$ gewählt werden, damit sich die Raumdiagonalen **senkrecht** schneiden?

---

## Lösungsweg

### Schritt 1: Koordinaten festlegen

Wir legen den Quader ins Koordinatensystem mit:

$$A(0\mid0\mid0), \quad G(4\mid3\mid h)$$

Die vier Raumdiagonalen verbinden jeweils gegenüberliegende Ecken. Wir betrachten die zwei Hauptdiagonalen:

- $\vec{d_1}$: von $A(0|0|0)$ nach $G(4|3|h)$
- $\vec{d_2}$: von $B(4|0|0)$ nach $H(0|3|h)$

---

### Schritt 2: Richtungsvektoren der Diagonalen

$$\vec{d_1} = \begin{pmatrix}4\\3\\h\end{pmatrix} \qquad \vec{d_2} = \begin{pmatrix}0-4\\3-0\\h-0\end{pmatrix} = \begin{pmatrix}-4\\3\\h\end{pmatrix}$$

---

### Schritt 3: Bedingung für Senkrechtstehen

Zwei Vektoren stehen senkrecht aufeinander, wenn ihr **Skalarprodukt = 0** ist:

$$\vec{d_1} \cdot \vec{d_2} = 0$$

$$\begin{pmatrix}4\\3\\h\end{pmatrix} \cdot \begin{pmatrix}-4\\3\\h\end{pmatrix} = 0$$

$$4 \cdot (-4) + 3 \cdot 3 + h \cdot h = 0$$

$$-16 + 9 + h^2 = 0$$

$$h^2 = 7$$

$$\boxed{h = \sqrt{7} \approx 2{,}65}$$

---

### Probe / Überprüfung

$$\vec{d_1} \cdot \vec{d_2} = -16 + 9 + 7 = 0 ✓$$

---

## Ergebnis

Die Höhe muss $h = \sqrt{7} \approx 2{,}65$ LE betragen, damit sich die Raumdiagonalen des Quaders senkrecht schneiden.
