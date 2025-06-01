# Geometrische Funktionen verschieben und Strecken

## Bedeutung der unterschiedlichen Werte in der allgemeinen Darstellung der Fuktion 

Die allgemeine Darstellung der sin-Funktion ist

$f(x)=a \cdot sin(b \cdot (x-d))+e$

??? tip "Liegt die Gleichung nicht in der gewünschten Form vor?"

    Manchmal wird die Funktion auch in der Form

    $f(x)=a \cdot sin(b_2x-d_2))+e$

    dargestellt. Um in die gewünschte Form zu kommen, musst du nur den Faktor
    $b_2$ herausziehen:

    $b_2 \cdot (x - \frac{d_2}{b_2})$

    sozusagen das Gegenteil von Ausmultiplizieren!
    
Dabei ist

### a = Streckung bzw. Stauchung in Y-Richtung

Werte über 1 entsprechen einer Streckung, Werte unter 1 einer Stauchung
Negative Werte entsprechen einer Spiegelung an der X-Achse bzw. an der zur
X-Achse parallelen Symmetrieachse, die sich ggf. durch eine Verschiebung ergibt.

### b = Streckung bzw. Stauchung in X-Richtung

Werte über 1 entsprechen hier einer Stauchung! Werte unter eins einer Streckung
Negative Werte entsprechen einter Spiegelung an der X-Achse

### d = Verschiebung in X-Richtung

Positive Werte verschieben die Funktion nach links, negative Werte nach rechts

### e = Verschiebung in Y-Richtung

Positive Werte verschieben die Funktion nach oben

## Herleitung der Funktion, wenn ein Hoch- und ein Tiefpunkt gegeben ist

Beispiel: Gegeben sind die Punkte

$T(\pi|-2)$ (Tiefpunkt)

$H(3\pi|6)$ (Hochpunkt)

### Verschiebung in Y-Richtung (e)

Der Hochpunkt und der Tiefpunkt sind auf der Y-Achse 8 Einheiten auseinander ($6 - (-2) = 8$)
Beide Punkte sind also 4 Einheiten von der neuen Mittelachse entfernt und die Mittelachse der Funktion liegt
also bei $y=2$ ($-2+4=2$ und $6-4=2$) damit ist

$e=2$

### Streckung in Y-Richtung (a)

Wie bereits berechnet, sind Hoch- und Tiefpunkt 4 Einheiten von der Mittelachse entfernt. Gegenüber der normalen
sin-Funktion ergibt sich damit direkt der Streckungsfaktor 4.

$a=4$

### Streckung in X-Richtung (b)

Hoch- und Tiefpunkt liegen auf der X-Achse $2\pi$ auseinander. Damit ergibt sich eine Periodenlänge von $4\pi$.
Gegenüber der normalen Periodenlänge von $2\pi$ haben wir also den Faktor 2. Für den Wert b müssen wir dann noch
den Kehrwert berechnen. Damit ist

$b=\frac{1}{2}$

### Verschiebung in X-Richtung (d)

Wir haben oben gezeigt, dass die Periodenlänge der Funktion $4\pi$ beträgt bzw. wir eine Streckung
um den Faktor 2 haben. Damit alleine würde sich für den ersten Hochpunkt (normalerweise bei $\frac{1}{2}\pi$) ein
X-Wert von $2\cdot \frac{1}{2} \pi = \pi$ ergeben. Unser Hochpunkt soll aber bei $3\pi$ liegen. Wir benötigen also
noch eine Verschiebung von

$d=2\pi$

wobei wir darauf achten müssen, dass der Wert abgezogen werden muss.

Damit ergibt sich für die Funktion:

$4\cdot \sin(\frac{1}{2}\cdot (x-2\pi))+2$

Alternativ kann die gleiche Funktion auch gespiegelt angegeben werden und dann die Verschiebung um eine halbe
Periodenlänge zurückgenommen werden - womit diese dann entfällt:

$-4\cdot \sin(\frac{1}{2}\cdot x)+2$

