# Die Flächeninhaltsfunktion der Normalparabel

Mittels der Streifenmethode und der Berechnung des Grenzwertes haben wir bereits die Fläche der Funktion

$$f(x)=x^2$$

im Intervall I=[0,1] berechnet. Nun können wir auf die gleiche Weise eine allgemeine Funktion zur Berechnung der Fläche
im Intervall I=[0,x] ermitteln.

$$\lim_{n \to \infty} O_{n}= \frac{1x}{n} \left( \left(\frac{1x}{n}\right)^2 + \left(\frac{2x}{n}\right)^2 + \left(\frac{3x}{n}\right)^2 ... \left(\frac{nx}{n}\right)^2 \right)$$

$$\lim_{n \to \infty} O_{n}= \frac{x}{n} \left( \left(\frac{x}{n}\right)^2 + \left(2\frac{x}{n}\right)^2 + \left(3\frac{x}{n}\right)^2 ... \left(n\frac{x}{n}\right)^2 \right)$$


wir haben hier also nur den Faktor x hinzugefügt. Nun können wir den Faktor $\left(\frac{x}{n}\right)^2 = \frac{x^2}{n^2}$ ebenfalls vor die Klammer ziehen

$$\lim_{n \to \infty} O_{n}= \frac{x}{n} \frac{x^2}{n^2} \left( 1^2 + 2^2 + 3^2 ... n^2\right)$$

nun können wir auch hier die Summenformel für Quadratzahlen einsetzen:

??? Tip "Summenformel für Quadratzahlen"

    $$1^2+2^2+3^2+4^2+...+n^2 = \sum_{k=1}^n k^2 = \frac{n(n+1)(2n+1)}{6}$$

$$\lim_{n \to \infty} O_{n}= \frac{x^3}{n^3} \left( \frac{n(n+1)(2n+1)}{6} \right)$$

Das Gleiche können wir auch anders aufschreiben:

$$\lim_{n \to \infty} O_{n}= \frac{x^3}{6} \frac{n}{n}  \frac{n+1}{n} \frac{2n+1}{n}$$

$$\lim_{n \to \infty} O_{n}= \frac{x^3}{6} \cdot 1  \cdot 1 \cdot 2$$

$$\lim_{n \to \infty} O_{n}= \frac{1}{3}x^3$$

