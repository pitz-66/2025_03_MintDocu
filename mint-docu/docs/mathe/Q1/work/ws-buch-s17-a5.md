# Buch Seite 17 Aufgabe 5

Gesucht ist der Inhalt der Fläche zwischen dem Graphen von $f(x)=x^3$ und der x-Achse über dem Intervall [0;1]
Gehen Sie analog zum archimedichen Beispiel $f(x)=x^2$ (S.16) vor.

Benötigte Summenformel: $1^3+2^3+...+n^3=\frac{n^2(n+1)^2}{4}$

$O_n=\frac{1}{n}\cdot\left[(\frac{1}{n})^3+(\frac{2}{n})^3+...+(\frac{n}{n})^3 \right]$

$O_n = \frac{1}{n}\cdot\frac{n}{n^3}\cdot\left[ 1^3+2^3+...+n^3 \right]$

$O_n = \frac{1}{n}\cdot\frac{n}{n^3}\cdot \frac{n^2(n+1)^2}{4}$

$O_n = \frac{1}{n^3}\cdot\frac{n^2(n+1)^2}{4}$

$O_n = \frac{1}{n^3}\cdot\frac{n^2(n^2+2n+1)}{4}$

$O_n = \frac{1}{4}\cdot\frac{n^2(n^2+2n+1)}{n^3}$

$O_n = \frac{1}{4}\cdot\frac{(n^2+2n+1)}{n}$