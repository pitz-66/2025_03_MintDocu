# Aufgabe 14 – Windschiefe Geraden

## Aufgabenstellung

Zeigen Sie, dass die folgenden Geradenpaare **windschief** sind.

Zwei Geraden sind windschief, wenn sie:

1. **nicht parallel** sind (Richtungsvektoren nicht kollinear), **und**
2. **keinen Schnittpunkt** haben (das Gleichungssystem ist widersprüchlich)

---

## a) Geraden g und h

$$g: \vec{x} = \begin{pmatrix}1\\0\\1\end{pmatrix} + r \begin{pmatrix}1\\-1\\0\end{pmatrix} \qquad h: \vec{x} = \begin{pmatrix}0\\1\\0\end{pmatrix} + s \begin{pmatrix}0\\1\\1\end{pmatrix}$$

### Schritt 1: Parallelität prüfen

$$\begin{pmatrix}1\\-1\\0\end{pmatrix} = k \cdot \begin{pmatrix}0\\1\\1\end{pmatrix}$$

Aus Zeile I: $1 = k \cdot 0$ → **Widerspruch** → die Vektoren sind nicht kollinear.

??? success "g und h sind **nicht parallel** ✓"
    Da $1 = k \cdot 0$ nicht lösbar ist, sind die Richtungsvektoren nicht kollinear.

### Schritt 2: Schnittpunkt prüfen

$$\begin{pmatrix}1\\0\\1\end{pmatrix} + r \begin{pmatrix}1\\-1\\0\end{pmatrix} = \begin{pmatrix}0\\1\\0\end{pmatrix} + s \begin{pmatrix}0\\1\\1\end{pmatrix}$$

| Zeile | Gleichung |
|-------|-----------|
| I | $1 + r = 0$ |
| II | $0 - r = 1 + s$ |
| III | $1 = s$ |

Aus **I**: $r = -1$  
Aus **III**: $s = 1$  
**Probe in II**: $-(-1) = 1$ und $1 + 1 = 2$ → $1 \neq 2$ → **Widerspruch!**

??? success "g und h haben keinen Schnittpunkt ✓"
    Zeile II liefert $1 \neq 2$ → das Gleichungssystem ist widersprüchlich.

??? abstract "Ergebnis a)"
    Da g und h **weder parallel noch schneidend** sind, sind sie **windschief** ✓

---

## b) Geraden g und h

$$g: \vec{x} = \begin{pmatrix}1\\1\\-1\end{pmatrix} + r \begin{pmatrix}1\\2\\1\end{pmatrix} \qquad h: \vec{x} = \begin{pmatrix}0\\1\\1\end{pmatrix} + s \begin{pmatrix}1\\1\\1\end{pmatrix}$$

### Schritt 1: Parallelität prüfen

$$\begin{pmatrix}1\\2\\1\end{pmatrix} = k \cdot \begin{pmatrix}1\\1\\1\end{pmatrix}$$

Aus Zeile I: $k = 1$, aber Zeile II: $2 = 1 \cdot 1 = 1$ → **Widerspruch**

??? success "g und h sind **nicht parallel** ✓"
    $k=1$ aus Zeile I passt nicht zu Zeile II ($2 \neq 1$).

### Schritt 2: Schnittpunkt prüfen

$$\begin{pmatrix}1\\1\\-1\end{pmatrix} + r \begin{pmatrix}1\\2\\1\end{pmatrix} = \begin{pmatrix}0\\1\\1\end{pmatrix} + s \begin{pmatrix}1\\1\\1\end{pmatrix}$$

| Zeile | Gleichung |
|-------|-----------|
| I | $1 + r = s$ |
| II | $1 + 2r = 1 + s$ |
| III | $-1 + r = 1 + s$ |

Aus **II**: $2r = s \Rightarrow s = 2r$  
In **I** einsetzen: $1 + r = 2r \Rightarrow r = 1$, damit $s = 2$

**Probe in III**: $-1 + 1 = 0$ und $1 + 2 = 3$ → $0 \neq 3$ → **Widerspruch!**

??? success "g und h haben keinen Schnittpunkt ✓"
    Zeile III liefert $0 \neq 3$ → das Gleichungssystem ist widersprüchlich.

??? abstract "Ergebnis b)"
    Da g und h **weder parallel noch schneidend** sind, sind sie **windschief** ✓

---

## c) Geraden g und k

$$g: \vec{x} = \begin{pmatrix}1\\-1\\2\end{pmatrix} + r \begin{pmatrix}2\\2\\1\end{pmatrix} \qquad k: \vec{x} = \begin{pmatrix}3\\-3\\0\end{pmatrix} + s \begin{pmatrix}0\\3\\1\end{pmatrix}$$

### Schritt 1: Parallelität prüfen

$$\begin{pmatrix}2\\2\\1\end{pmatrix} = k \cdot \begin{pmatrix}0\\3\\1\end{pmatrix}$$

Aus Zeile I: $2 = k \cdot 0$ → **Widerspruch**

??? success "g und k sind **nicht parallel** ✓"
    $2 = 0$ ist nicht lösbar → Richtungsvektoren sind nicht kollinear.

### Schritt 2: Schnittpunkt prüfen

$$\begin{pmatrix}1\\-1\\2\end{pmatrix} + r \begin{pmatrix}2\\2\\1\end{pmatrix} = \begin{pmatrix}3\\-3\\0\end{pmatrix} + s \begin{pmatrix}0\\3\\1\end{pmatrix}$$

| Zeile | Gleichung |
|-------|-----------|
| I | $1 + 2r = 3$ |
| II | $-1 + 2r = -3 + 3s$ |
| III | $2 + r = s$ |

Aus **I**: $r = 1$  
Aus **III**: $s = 2 + 1 = 3$

**Probe in II**: $-1 + 2 = 1$ und $-3 + 9 = 6$ → $1 \neq 6$ → **Widerspruch!**

??? success "g und k haben keinen Schnittpunkt ✓"
    Zeile II liefert $1 \neq 6$ → das Gleichungssystem ist widersprüchlich.

??? abstract "Ergebnis c)"
    Da g und k **weder parallel noch schneidend** sind, sind sie **windschief** ✓

---

## Gesamtzusammenfassung

!!! abstract "Alle Ergebnisse"

    | Teilaufgabe | Nicht parallel? | Kein Schnittpunkt? | Windschief? |
    |-------------|:-:|:-:|:-:|
    | **a) g und h** | ✓ | ✓ | **✓ windschief** |
    | **b) g und h** | ✓ | ✓ | **✓ windschief** |
    | **c) g und k** | ✓ | ✓ | **✓ windschief** |

!!! tip "Merksatz"
    Zwei Geraden im $\mathbb{R}^3$ sind **windschief**, wenn sie weder parallel sind noch einen gemeinsamen Punkt besitzen. Dies ist ein Phänomen, das im $\mathbb{R}^2$ (in der Ebene) nicht existiert!
