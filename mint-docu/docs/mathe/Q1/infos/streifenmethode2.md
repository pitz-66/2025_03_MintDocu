# Die Streifenmethode des Archimedes, zweite Seite

## Zweites Beispiel

### Gegeben ist die Funktion

$$f(x)=x+1$$

im Intervall [0..1]

Die __Obersumme__ für n=4

$$O_{4} = \frac{1}{4}\frac{5}{4} + \frac{1}{4}\frac{6}{4} + \frac{1}{4}\frac{7}{4} + \frac{1}{4}\frac{8}{4}$$

$$O_{4} = \frac{5}{16} + \frac{6}{16} + \frac{7}{16} + \frac{8}{16}$$

$$O_{4} = \frac{26}{16} = \frac{13}{8} = 1.625$$

Die __Untersumme__ für n=4

$$O_{4} = \frac{1}{4} + \frac{1}{4}\frac{5}{4} + \frac{1}{4}\frac{6}{4} + \frac{1}{4}\frac{7}{4}$$

$$O_{4} = \frac{4}{16} + \frac{5}{16} + \frac{6}{16} + \frac{7}{16}$$

$$O_{4} = \frac{22}{16} = \frac{11}{8} = 1.375$$

Der Mittelwert liegt damit bei $\frac{12}{8}=\frac{3}{2}=1.5$ was in diesem Fall sogar genau der Fläche entspricht.


### Grenzwertbetrachtung

$$\lim_{n \to \infty} O_{n}=\frac{1}{n} \left( \left(1+\frac{1}{n}\right) + \left(1+\frac{2}{n}\right) + \left(1+\frac{3}{n}\right) ... \left(1+\frac{n}{n}\right) \right)$$

Den Faktor $\frac{1}{n}$ ziehen wir durch Ausmultiplizieren in die Klammer

$$\lim_{n \to \infty} O_{n}= \left(\frac{1}{n}+\frac{1}{n^2}\right) + \left(\frac{1}{n}+\frac{2}{n^2}\right) + \left(\frac{1}{n}+\frac{3}{n^2}\right) ... \left(\frac{1}{n}+\frac{n}{n^2}\right)$$

Da nun der Summand $\frac{1}{n}$ genau n mal vorkommt können entsprechend vereinfachen $n \frac{1}{n} = 1$

$$\lim_{n \to \infty} O_{n}= 1 + \frac{1}{n^2} + \frac{2}{n^2} + \frac{3}{n^2} ... \frac{1}{n^2}$$

oder, da alle Summanden den gleichen Quotienten haben

$$\lim_{n \to \infty} O_{n}= 1 + \frac{1+2+3...n}{n^2}$$

Und nun verwenden wie die Gaußsche Summenformel!

??? Tip "Gaußsche Summenformel"

    $$1+2+3+4+5+...+n = \sum_{k=1}^n k = \frac{n(n+1)}{2}$$

$$\lim_{n \to \infty} O_{n}= 1 + \frac{n(n+1)}{2n^2}$$

$$\lim_{n \to \infty} O_{n}= 1 + \frac{n^2+n}{2n^2}$$

$$\lim_{n \to \infty} O_{n}= 1 + \frac{n^2}{2n^2} + \frac{n}{2n^2}$$

$$\lim_{n \to \infty} O_{n}= 1 + \frac{1}{2} + \frac{1}{2n}$$

$$\lim_{n \to \infty} O_{n}= \frac{3}{2}$$