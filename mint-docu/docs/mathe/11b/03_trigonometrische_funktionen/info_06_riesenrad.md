# Das Riesenrad

siehe auch Mathebuch Seite 245 Aufgabe 3

3) Das Riesenrad hat einen Durchmesser von 60m und dreht sich einmal in 20 Sekunden. Der
tiefste Punkt liegt 3m über dem Straßenniveau.

3a) Herleitung der Funktion

!!! tip "Cosinus statt Sinus"

    Unsere Gondel startet im Tiefsten Punkt der Funktion. Die Sinus-Funktion hat allerdings
    im Ursprung einen Wendepunkt! Die Cosinus-Funktion hat im Ursprung einen Hochpunkt. Dies
    können wir aber sehr einfach durch eine Spiegelung zu einem Tiefpunkt machen.

    Mann könnte nun zwar eine Sinus-Funktion entsprechend Verschieben, die Herleitung der
    Verschiebung ist allerding nicht einfach, da wir ja eigentlich immer nur den Ursprung bei
    der Verschiebung betrachen und wir - wenn wir den Tiefpunkt in den Ursprung verschieben
    wollen, auch die Streckung der Funktion berücksichtigen müssen.

$f(x)= a \cdot (-cos(b(x-d))) + e$

Aus dem Radius (30m) und der Lage 3m über Straßenniveau ergibt sich eine Verschiebung auf der
Y-Achse von 33m:

$e=33$

Aus dem Radius von 30m ergibt sich direkt die Streckung in Y-Richtung

$a=30$

Aus der Zeit von 20s für einen Umlauf können wir eine Periodenlänge von 20 ableiten. Die
Streckung beträgt also $\frac{20}{2\pi}$, der Wert für b ist der Umkehrwert und damit

$b=\frac{pi}{10}$

Eine Verschiebung in X-Richtung brauchen wir nicht zu beachten, da ja unser Tiefpunkt bereits
im Ursprung liegt. Damit ergibt sich

$f(x)= 30 \cdot (-cos(\frac{pi}{10} \cdot x)) + 33$

oder

$f(x)=33 - 30 \cdot cos(\frac{pi}{10} \cdot x)$

