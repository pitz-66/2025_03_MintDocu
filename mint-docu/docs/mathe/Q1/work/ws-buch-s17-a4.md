# Buch Seite 17 Aufgabe 4

Berechnen Sie $U_n$ und $O_n$ für die Funktion f über dem Intervall I.

Welcher Grenzwert ergibt sich jeweils für $\lim_{n}^\infty$

!!! Tip "Benötigete Summenformeln"

    $1+2+...+n=\frac{n(n+1)}{2}$

    $1^2+2^2+...+n^2=\frac{n(n+1)(2n+1)}{6}$

### a) $f(x)=x+1$ im Intervall $I=[0;1]$

$U_n = \frac{1}{n}\cdot\left[ (0+1)+(\frac{1}{n}+1)+ (\frac{2}{n}+1)+...+(\frac{n-1}{n}+1)\right]$

$U_n = \frac{1}{n}\cdot n + \frac{1}{n}\cdot\left[ 0+\frac{1}{n}+ \frac{2}{n}+...+\frac{n-1}{n}\right]$

$U_n = 1 + \frac{1}{n^2}\cdot\left[ 0+1+2+...+{n-1}\right]$

$U_n = 1 + \frac{1}{n^2}\cdot \left( \frac{n(n+1)}{2} -1\right)$

$U_n = 1 + \frac{n(n+1)}{2n^2} -\frac{1}{n^2}$

$U_n = 1 + \frac{n(n+1)}{2n^2} -\frac{1}{n^2}$

$U_n = 1 + \frac{n^2+n}{2n^2} -\frac{1}{n^2}$

$U_n = 1 + \frac{n^2}{2n^2} + \frac{n}{2n^2} -\frac{1}{n^2}$

$U_n = 1 + \frac{1}{2} + \frac{1}{2n} -\frac{1}{n^2}$

$\lim_{n}^\infty U_n= \frac{3}{2}$

---

### b) $f(x)=2-x$ im Intervall $I=[0;2]$

$O_n= \frac{2}{n} \cdot \left[ (2-\frac{2}{n}) +  (2-\frac{4}{n})+ ... + (2-\frac{2n}{n})\right]$

$O_n= \frac{2}{n} \cdot 2n -\frac{2}{n} \cdot \left[ (\frac{2}{n}) +  (\frac{4}{n})+ ... + (\frac{2n}{n})\right]$

$O_n= \frac{2}{n} \cdot 2n -\frac{4}{n^2} \cdot \left[ 1 + 2 + ... + n \right]$

$O_n= \frac{2}{n} \cdot 2n -\frac{4}{n^2} \cdot \frac{n(n+1)}{2}$

$O_n= 4 - \frac{4n^2+4n}{2n^2} =  4 - \frac{4n^2}{2n^2} - \frac{4n}{2n^2} = 4 - 2 - \frac{2}{n}$

$\lim_{n}^\infty O_n= 2$

---

### c) $f(x)=x^2$ im Intervall $I=[0;10]$

$U_n=\frac{10}{n}\cdot\left[ 0+(\frac{10}{n})^2+(\frac{2\cdot10}{n})^2+...+(\frac{(n-1)\cdot10}{n})^2 \right]$

$U_n=\frac{10}{n}\cdot\frac{100}{n^2}\cdot\left[ 0^2+1^2+2^2+...+(n-1)^2 \right]$

$U_n=\frac{1000}{n^3}\cdot\left[ 0^2+1^2+2^2+...+(n-1)^2 \right]$

$U_n=\frac{1000}{n^3}\cdot\left[ \frac{(n-1)n(2n-1)}{6} \right]$

$U_n=\frac{1000}{n^3}\cdot\left[ \frac{2n^3-3n^2+n}{6} \right]$

$U_n=\frac{1000}{6}\cdot\left[ \frac{2n^3}{n^3}-\frac{3n^2}{n^3}+\frac{n}{n^3} \right]$

$U_n=\frac{1000}{6}\cdot\left[ 2-\frac{3}{n}+\frac{1}{n^2} \right]$

$\lim_{n}^\infty U_n= \frac{1000}{6}\cdot 2 = \frac{1000}{3}$

---

### d) $f(x)=2x^2+x$ im Intervall $I=[0;1]$

$O_n=\frac{1}{n}\cdot\left[ 2(\frac{1}{n})^2+\frac{1}{n} + 2(\frac{2}{n})^2+\frac{2}{n} + ... + 2(\frac{n}{n})^2+\frac{n}{n} \right]$

$O_n=\frac{1}{n}\cdot\left[ \frac{2}{n^2} + \frac{1}{n} + \frac{8}{n^2} + \frac{2}{n} + ... + 2 + 1 \right]$

$O_n=\frac{1}{n}\cdot\left[ \frac{2}{n^2}(1^2+2^2+...+n^2) + \frac{1}{n}(1+2+...+n) \right]$

$O_n=\frac{1}{n}\cdot\left[ \frac{2}{n^2}\cdot\frac{n(n+1)(2n+1)}{6} + \frac{1}{n}\cdot\frac{n(n+1)}{2} \right]$

$O_n=\frac{1}{n}\cdot\left[ \frac{2(2n^3+3n^2+n)}{6n^2} + \frac{n(n+1)}{2n} \right]$

$O_n=\frac{1}{n}\cdot\left[ \frac{2(2n^3+3n^2+n)}{6n^2} + \frac{3n^2(n+1)}{6n^2} \right]$

$O_n=\frac{1}{n}\cdot\left[ \frac{4n^3+6n^2+2n + 3n^3+3n^2}{6n^2} \right]$

$O_n=\frac{1}{n}\cdot\left[ \frac{7n^3+9n^2+2n}{6n^2} \right]$

$O_n=\frac{7n^3+9n^2+2n}{6n^3} = \frac{7n^3}{6n^3} + \frac{9n^2}{6n^3} + \frac{2n}{6n^3}$

$O_n=\frac{7}{6} + \frac{3}{2n} + \frac{1}{3n^2}$

$\lim_{n}^\infty O_n= \frac{7}{6}$
