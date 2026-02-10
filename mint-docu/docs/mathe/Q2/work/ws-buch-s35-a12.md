# Buch S. 35, Aufgabe 12

## **Gegeben**

Die Wurfparabel lautet:

$$
h(t) = a t^2 + b t + c
$$

Punkte des Fluges:

1.  Start: $h(0) = 1$
2.  Nach 0,5s: $h(0{,}5) = 2{,}75$
3.  Nach 1s: $h(1) = 2$

## a) Bestimmung der Koeffizienten a, b, c

### 1. Gleichungen aufstellen

#### Aus $h(0)=1$:

$a\cdot 0^2 + b\cdot 0 + c = 1$

$\Rightarrow c = 1$

#### Aus $h(0{,}5)=2{,}75$:

$a(0{,}5)^2 + b(0{,}5) + 1 = 2{,}75$

$0{,}25a + 0{,}5b = 1{,}75$

#### Aus $h(1)=2$:

$a + b + 1 = 2$

$a + b = 1$

Damit entsteht das lineare Gleichungssystem:

$$
\begin{cases}
0{,}25a + 0{,}5b = 1{,}75 \\
a + b = 1 \\
c=1
\end{cases}
$$

### 2. Gaußscher Eliminationsalgorithmus

Wir lösen:

$$
\begin{pmatrix}
0.25 & 0.5 & | & 1.75 \\
1 & 1 & | & 1
\end{pmatrix}
$$

#### 1. Pivot normalisieren:

Multipliziere Zeile 1 mit 4:

$$
\begin{pmatrix}
1 & 2 & | & 7 \\
1 & 1 & | & 1
\end{pmatrix}
$$

#### 2. Eliminiere a in Zeile 2

$Z_2 \leftarrow Z_2 - Z_1$

$$
\begin{pmatrix}
1 & 2 & | & 7 \\
0 & -1 & | & -6
\end{pmatrix}
$$

#### 3. Nach b auflösen

$-b = -6 \quad\Rightarrow\quad b = 6$

#### 4. Rückeinsetzen in $a + b = 1$

$a + 6 = 1 \Rightarrow a = -5$

## ✅ *Lösung Teil a)*

$\boxed{a = -5,\quad b = 6,\quad c = 1}$

Damit lautet die Höhenfunktion:

$\boxed{h(t) = -5t^2 + 6t + 1}$

## *b) Wann trifft der Ball den Boden?*

Wir suchen den Zeitpunkt, bei dem $h(t)=0$:

$$
-5t^2 + 6t + 1 = 0
$$

Die Formel

$$
h(t)= -5t^2 + 6t + 1
$$

muss für $h(t)=0$ gelöst werden. Dafür formt man sie nur zur passenden pq‑Form um.

***

### ⭐ Kurz: Was ist die pq‑Formel?

Die **pq‑Formel** löst quadratische Gleichungen der Form

$$
t^2 + p t + q = 0.
$$

Die Lösungen lauten:

$$
t = -\frac{p}{2} \pm \sqrt{\left(\frac{p}{2}\right)^2 - q}.
$$

Sie ist praktisch eine vereinfachte Version der Mitternachtsformel, wenn der Leitkoeffizient (vor $t^2$) **1** ist.


## ⭐ Teil b mit der pq‑Formel lösen

Unsere Gleichung lautet:

$$
-5t^2 + 6t + 1 = 0.
$$

Zuerst auf die Form $t^2 + pt + q = 0$ bringen:

$$
t^2 - \frac{6}{5}t - \frac{1}{5} = 0.
$$

Damit sind:

$$
p = -\frac{6}{5}, \qquad q = -\frac{1}{5}.
$$

Jetzt die pq‑Formel anwenden:

$$
t = -\frac{p}{2} \pm \sqrt{\left(\frac{p}{2}\right)^2 - q}.
$$

Einsetzen:

1.  $\displaystyle -\frac{p}{2} = -\left(-\frac{6}{5} \cdot \frac12\right) = \frac{3}{5}$
2.  $\displaystyle \left(\frac{p}{2}\right)^2 = \left(-\frac{3}{5}\right)^2 = \frac{9}{25}$
3.  $-q = \frac{1}{5} = \frac{5}{25}$

Unter der Wurzel:

$$
\frac{9}{25} + \frac{5}{25} = \frac{14}{25}
$$

Somit:

$$
t = \frac{3}{5} \pm \sqrt{\frac{14}{25}}
$$

$$
t = \frac{3}{5} \pm \frac{\sqrt{14}}{5}
$$

Also:

$$
t = \frac{3 + \sqrt{14}}{5}
\quad\text{oder}\quad 
t = \frac{3 - \sqrt{14}}{5}
$$

Die **positive physikalisch sinnvolle Lösung** ist:

$$
t = \frac{3 + \sqrt{14}}{5} \approx 1{,}48\ \text{s}.
$$

***

# ✅ Ergebnis

Die Zeit, bis der Ball den Boden berührt, beträgt:

$$
\boxed{t \approx 1{,}48\ \text{Sekunden}}
$$
