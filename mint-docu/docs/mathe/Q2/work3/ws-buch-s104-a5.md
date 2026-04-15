# Aufgabe 5 – Bogenschießen

## Aufgabenstellung

Ein Bogenschütze steht am Punkt $P(0|0|15)$ und zielt in Richtung des Vektors:

$$\vec{v} = \begin{pmatrix}-1\\3\\0{,}5\end{pmatrix}$$

Im Bergland sind drei Scheiben aufgestellt:

| Scheibe | Koordinaten |
|---------|-------------|
| 🐻 **Bär** | $B(-155 \mid 465 \mid 85)$ |
| 🐺 **Wolf** | $W(-155 \mid 465 \mid 92{,}5)$ |
| 🫎 **Elch** | $E(-160 \mid 640 \mid 95)$ |

> **Maßstab:** $1 \text{ LE} = 1 \text{ dm}$

**a)** Welche Scheibe trifft der Schütze? Wie lang ist die Flugbahn?  
Welche Geschwindigkeit hat der Pfeil, wenn der Flug eine Sekunde dauert?

**b)** In welche Richtung $\vec{w}$ muss der Schütze zielen, um die **Elchscheibe** zu treffen?

---

## Lösung

### Schritt 1: Geradengleichung der Flugbahn aufstellen

Die Flugbahn des Pfeils ist eine Gerade durch $P$ in Richtung $\vec{v}$:

$$g: \vec{x} = \begin{pmatrix}0\\0\\15\end{pmatrix} + t \cdot \begin{pmatrix}-1\\3\\0{,}5\end{pmatrix}$$

---

### Teil a) Welche Scheibe wird getroffen?

Wir prüfen für jede Scheibe, ob sie auf der Geraden $g$ liegt, indem wir das Gleichungssystem lösen.

---

#### 🐻 Bär $B(-155 \mid 465 \mid 85)$

$$\begin{pmatrix}-155\\465\\85\end{pmatrix} = \begin{pmatrix}0\\0\\15\end{pmatrix} + t \cdot \begin{pmatrix}-1\\3\\0{,}5\end{pmatrix}$$

| Zeile | Gleichung | Ergebnis |
|-------|-----------|----------|
| I | $-1 \cdot t = -155$ | $t = 155$ |
| II | $3 \cdot t = 465$ | $t = 155$ |
| III | $15 + 0{,}5 \cdot t = 85$ | $t = 140$ |

??? failure "Bär wird **nicht** getroffen"
    Zeile III liefert $t = 140 \neq 155$ → **Widerspruch**.  
    Der Pfeil verfehlt die Bär-Scheibe.

---

#### 🐺 Wolf $W(-155 \mid 465 \mid 92{,}5)$

$$\begin{pmatrix}-155\\465\\92{,}5\end{pmatrix} = \begin{pmatrix}0\\0\\15\end{pmatrix} + t \cdot \begin{pmatrix}-1\\3\\0{,}5\end{pmatrix}$$

| Zeile | Gleichung | Ergebnis |
|-------|-----------|----------|
| I | $-1 \cdot t = -155$ | $t = 155$ |
| II | $3 \cdot t = 465$ | $t = 155$ |
| III | $15 + 0{,}5 \cdot t = 92{,}5$ | $t = 155$ |

??? success "Wolf wird **getroffen** ✓"
    Alle drei Gleichungen liefern $t = 155$ → **kein Widerspruch**.  
    Der Pfeil trifft die **Wolf-Scheibe**.

---

#### Flugbahnlänge

Der Pfeil fliegt vom Punkt $P$ bis zum Punkt $W$, also den Vektor:

$$\vec{PW} = t \cdot \vec{v} = 155 \cdot \begin{pmatrix}-1\\3\\0{,}5\end{pmatrix} = \begin{pmatrix}-155\\465\\77{,}5\end{pmatrix}$$

Die **Länge der Flugbahn** ist der Betrag dieses Vektors:

$$|\vec{PW}| = |t| \cdot |\vec{v}| = 155 \cdot \sqrt{(-1)^2 + 3^2 + 0{,}5^2}$$

$$= 155 \cdot \sqrt{1 + 9 + 0{,}25} = 155 \cdot \sqrt{10{,}25} \approx 155 \cdot 3{,}202$$

$$\approx 496{,}3 \text{ LE} = 496{,}3 \text{ dm} \approx \mathbf{49{,}6 \text{ m}}$$

#### Geschwindigkeit des Pfeils

Bei einer Flugdauer von $t = 1$ Sekunde gilt:

$$v = \frac{\text{Strecke}}{\text{Zeit}} = \frac{496{,}3 \text{ dm}}{1 \text{ s}} = 496{,}3 \frac{\text{dm}}{\text{s}} \approx \mathbf{49{,}6 \frac{\text{m}}{\text{s}}}$$

??? note "Ergebnis Teil a)"
    - Der Schütze trifft die **Wolf-Scheibe** 🐺
    - Die Flugbahn ist ca. $\mathbf{496{,}3 \text{ dm} \approx 49{,}6 \text{ m}}$ lang
    - Die Geschwindigkeit des Pfeils beträgt ca. $\mathbf{49{,}6 \frac{m}{s} \approx 179 \frac{km}{h}}$

---

### Teil b) Richtungsvektor $\vec{w}$ zur Elch-Scheibe

Der Schütze steht weiterhin in $P(0|0|15)$ und möchte die Elch-Scheibe $E(-160|640|95)$ treffen.

Der gesuchte Richtungsvektor $\vec{w}$ zeigt von $P$ nach $E$:

$$\vec{w} = E - P = \begin{pmatrix}-160 - 0\\640 - 0\\95 - 15\end{pmatrix} = \begin{pmatrix}-160\\640\\80\end{pmatrix}$$

Wir vereinfachen durch Division durch $80$:

$$\vec{w} = 80 \cdot \begin{pmatrix}-2\\8\\1\end{pmatrix}$$

Als normierter Richtungsvektor (ohne Skalierung):

$$\vec{w} = \begin{pmatrix}-2\\8\\1\end{pmatrix}$$

**Probe:** Liegt $E$ auf der Geraden $P + t \cdot \vec{w}$?

$$\begin{pmatrix}0\\0\\15\end{pmatrix} + 80 \cdot \begin{pmatrix}-2\\8\\1\end{pmatrix} = \begin{pmatrix}-160\\640\\95\end{pmatrix} \checkmark$$

??? success "Ergebnis Teil b)"
    Der Schütze muss in Richtung

    $$\vec{w} = \begin{pmatrix}-2\\8\\1\end{pmatrix}$$

    zielen, um die **Elch-Scheibe** 🫎 zu treffen.

---

## Gesamtzusammenfassung

!!! abstract "Alle Ergebnisse auf einen Blick"

    | Teilaufgabe | Ergebnis |
    |-------------|----------|
    | **Getroffene Scheibe** | Wolf 🐺 bei $t = 155$ |
    | **Flugbahnlänge** | $\approx 496{,}3 \text{ dm} \approx 49{,}6 \text{ m}$ |
    | **Geschwindigkeit** | $\approx 49{,}6 \frac{\text{m}}{\text{s}} \approx 179 \frac{\text{km}}{\text{h}}$ |
    | **Richtung für Elch** | $\vec{w} = \begin{pmatrix}-2\\8\\1\end{pmatrix}$ |
