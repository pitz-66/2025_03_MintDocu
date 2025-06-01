# Hoch und Tiefpunkte von trigonometrischen Funktionen

??? tip "...gute Erklärung dazu in Youtube :-)"

    [https://www.youtube.com/watch?v=fYDhjLxM5sM](https://www.youtube.com/watch?v=fYDhjLxM5sM)

## Generelles Vorgehen:

1. Erste und Zeite Ableitung bilden
2. Nullstellen der ersten Ableitung Finden, dort liegen die Extrempunkte
3. Einsetzen in zweite Ableitung, Werte kleiner Null für einen Hochpunkt,
   größer Null für einen Tiefpunkt
4. ggf. Periode ausrechnen



## Beispiel

$f(x)=\frac{3}{2} \cdot \sin(\frac{\pi}{3} \cdot (x-1))+1$

Für die Ableitungen benötigen wir die Kettenregel:

$f(x)=u(v(x)) \to f'(x)=u'(v(x)) \cdot v'(x)$

Erste Ableitung

$f'(x)=\frac{3}{2} \cdot cos(\frac{\pi}{3} \cdot (x-1)) \cdot \frac{\pi}{3}$

$f'(x)=\frac{\pi}{2} \cdot cos(\frac{\pi}{3} \cdot (x-1))$

Zweite Ableitung

$f''(x)=\frac{\pi}{2} \cdot (-\sin(\frac{\pi}{3} \cdot (x-1))) \cdot \frac{\pi}{3}$

$f''(x)=-\frac{\pi^2}{6} \cdot \sin(\frac{\pi}{3} \cdot (x-1))$

Erste Ableitung gleich Nullsetzen:

$0=\frac{\pi}{2} \cdot cos(\frac{\pi}{3} \cdot (x-1))$

$0=cos(\frac{\pi}{3} \cdot (x-1))$

!!! tip "im Taschenrechner RAD-Maß verwenden!"

$\arccos(0)=\frac{\pi}{3} \cdot (x-1)$

$\frac{\pi}{2} = \frac{\pi}{3} \cdot (x-1)$

$\frac{3}{2} = x-1$

$\frac{5}{2} = x_1$

Zweite Lösung:


Verschieben in den positiven Bereich:

