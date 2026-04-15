# Übung 3 – Parallele Geraden

## Aufgabe

Welche der folgenden Geraden sind **parallel**, welche **schneiden sich**?

**Gerade g:**

$$\vec{x} = \begin{pmatrix}1\\0\\2\end{pmatrix} + r \begin{pmatrix}2\\-1\\1\end{pmatrix}$$

**Gerade h:**

$$\vec{x} = \begin{pmatrix}5\\-3\\2\end{pmatrix} + s \begin{pmatrix}-2\\3\\3\end{pmatrix}$$

**Gerade u** durch $C(2|-2|3)$ und $D(-2|0|1)$

**Gerade v** durch $E(2|0|0)$ und $F(0|3|3)$

---

## Schritt 1: Richtungsvektoren bestimmen

Für **g** und **h** sind die Richtungsvektoren bereits gegeben:

$$\vec{r}_g = \begin{pmatrix}2\\-1\\1\end{pmatrix}, \qquad \vec{r}_h = \begin{pmatrix}-2\\3\\3\end{pmatrix}$$

Für **u** und **v** berechnen wir sie aus den Punkten:

$$\vec{r}_u = D - C = \begin{pmatrix}-2-2\\0-(-2)\\1-3\end{pmatrix} = \begin{pmatrix}-4\\2\\-2\end{pmatrix}$$

$$\vec{r}_v = F - E = \begin{pmatrix}0-2\\3-0\\3-0\end{pmatrix} = \begin{pmatrix}-2\\3\\3\end{pmatrix}$$

---

## Schritt 2: Parallelität prüfen

Zwei Geraden sind parallel, wenn ihre Richtungsvektoren **kollinear** sind, d.h. $\vec{r}_1 = k \cdot \vec{r}_2$.

### g ∥ u ?

$$\vec{r}_u = \begin{pmatrix}-4\\2\\-2\end{pmatrix} = k \cdot \begin{pmatrix}2\\-1\\1\end{pmatrix}$$

Aus der ersten Komponente: $k = -2$. Probe:

$$-2 \cdot \begin{pmatrix}2\\-1\\1\end{pmatrix} = \begin{pmatrix}-4\\2\\-2\end{pmatrix} \checkmark$$

!!! success "g ∥ u"
    Die Richtungsvektoren sind kollinear mit $k = -2$.  
    **Geraden g und u sind parallel.**  
    Nun prüfen wir noch, ob sie identisch sind, indem wir testen, ob $C$ auf $g$ liegt:

    $$\begin{pmatrix}2\\-2\\3\end{pmatrix} = \begin{pmatrix}1\\0\\2\end{pmatrix} + r\begin{pmatrix}2\\-1\\1\end{pmatrix}$$

    Aus Zeile 1: $r = \frac{1}{2}$ | Zeile 2: $r = 2$ → **Widerspruch**

    g und u sind **echt parallel** (nicht identisch).

---

### h ∥ v ?

$$\vec{r}_v = \begin{pmatrix}-2\\3\\3\end{pmatrix} = k \cdot \begin{pmatrix}-2\\3\\3\end{pmatrix} \Rightarrow k = 1 \checkmark$$

!!! success "h ∥ v"
    Die Richtungsvektoren sind **identisch**.  
    **Geraden h und v sind parallel.**  
    Nun prüfen wir, ob sie identisch sind, indem wir testen ob $E(2|0|0)$ auf $h$ liegt:

    $$\begin{pmatrix}2\\0\\0\end{pmatrix} = \begin{pmatrix}5\\-3\\2\end{pmatrix} + s\begin{pmatrix}-2\\3\\3\end{pmatrix}$$

    Zeile 1: $s = \frac{3}{2}$ | Zeile 2: $s = 1$ → **Widerspruch**

    h und v sind **echt parallel** (nicht identisch).

---

## Schritt 3: Schnitt prüfen (g ∩ h und weitere Paare)

### g ∩ h ?

Gleichungssystem aufstellen ($\vec{x}_g = \vec{x}_h$):

$$\begin{pmatrix}1\\0\\2\end{pmatrix} + r\begin{pmatrix}2\\-1\\1\end{pmatrix} = \begin{pmatrix}5\\-3\\2\end{pmatrix} + s\begin{pmatrix}-2\\3\\3\end{pmatrix}$$

| Zeile | Gleichung |
|-------|-----------|
| I | $1 + 2r = 5 - 2s$ |
| II | $0 - r = -3 + 3s$ |
| III | $2 + r = 2 + 3s$ |

Aus **III**: $r = 3s$

Einsetzen in **II**: $-3s = -3 + 3s \Rightarrow -6s = -3 \Rightarrow s = \frac{1}{2}$, damit $r = \frac{3}{2}$

**Probe in I:** $1 + 2 \cdot \frac{3}{2} = 4$ und $5 - 2 \cdot \frac{1}{2} = 4$ ✓

**Schnittpunkt berechnen:**

$$\vec{x} = \begin{pmatrix}1\\0\\2\end{pmatrix} + \frac{3}{2}\begin{pmatrix}2\\-1\\1\end{pmatrix} = \begin{pmatrix}4\\-\frac{3}{2}\\\frac{7}{2}\end{pmatrix}$$

!!! info "g ∩ h"
    g und h **schneiden sich** im Punkt $S\!\left(4\ \Big|\ {-\tfrac{3}{2}}\ \Big|\ \tfrac{7}{2}\right)$.

---

### u ∩ v ?

Da **g ∥ u** und **h ∥ v**, verhalten sich u und v genauso wie g und h. Wir prüfen direkt:

Gerade u: Stützvektor $C(2|-2|3)$, Richtung $\begin{pmatrix}-4\\2\\-2\end{pmatrix}$ (bzw. $\begin{pmatrix}2\\-1\\1\end{pmatrix}$)

Gerade v: Stützvektor $E(2|0|0)$, Richtung $\begin{pmatrix}-2\\3\\3\end{pmatrix}$

$$\begin{pmatrix}2\\-2\\3\end{pmatrix} + r\begin{pmatrix}2\\-1\\1\end{pmatrix} = \begin{pmatrix}2\\0\\0\end{pmatrix} + s\begin{pmatrix}-2\\3\\3\end{pmatrix}$$

| Zeile | Gleichung |
|-------|-----------|
| I | $2 + 2r = 2 - 2s \Rightarrow r = -s$ |
| II | $-2 - r = 3s$ |
| III | $3 + r = 3s$ |

Aus I: $r = -s$, einsetzen in III: $3 - s = 3s \Rightarrow s = \frac{3}{4}$, $r = -\frac{3}{4}$

**Probe in II:** $-2 + \frac{3}{4} = -\frac{5}{4}$ und $3 \cdot \frac{3}{4} = \frac{9}{4}$ → **Widerspruch!**

!!! warning "u und v schneiden sich nicht"
    Da die Probe fehlschlägt und die Geraden **nicht parallel** sind, sind u und v **windschief**.

---

## Zusammenfassung

!!! abstract "Ergebnis"

    | Geradenpaar | Beziehung |
    |-------------|-----------|
    | **g und u** | echt parallel |
    | **h und v** | echt parallel |
    | **g und h** | schneiden sich in $S\!\left(4\ \big|\ {-\tfrac{3}{2}}\ \big|\ \tfrac{7}{2}\right)$ |
    | **u und v** | windschief |
