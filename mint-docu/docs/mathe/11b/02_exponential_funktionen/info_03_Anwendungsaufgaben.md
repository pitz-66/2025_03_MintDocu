# Anwendungsaufgaben

## Halbwertszeit

Bei einem exponentiellen Zerfall wird die Halbwertszeit als die Zeit definiert, in der die Hälfte der ursprünglichen Menge eines Stoffes zerfallen ist.
Für einen Zerfallsprozess mit der Funktion

$f(t) = c \cdot a^t$

gilt:

$T_{1/2} = \frac{\log(\frac{1}{2})}{\log(a)}$

wobei $T_{1/2}$ die Halbwertszeit, $c$ die Anfangsmenge und $a$ der Zerfallsfaktor ist.
Die Halbwertszeit ist also unabhängig von der Anfangsmenge $c$ und hängt nur vom Zerfallsfaktor $a$ ab.

??? tip "Beweis"

    $f(t) = c \cdot a^t$

    $f(T_{1/2}) = c \cdot a^{T_{1/2}} = \frac{c}{2}$

    $\Rightarrow a^{T_{1/2}} = \frac{1}{2}$

    $\Rightarrow log(a^{T_{1/2}}) = log(\frac{1}{2})$

    $\Rightarrow T_{1/2} \cdot log(a) = log(\frac{1}{2})$

    $\Rightarrow T_{1/2} = \frac{\log(\frac{1}{2})}{\log(a)}$

??? example "Beispiel"

    Ein radioaktives Element hat eine Halbwertszeit von 5 Jahren. Wenn zu Beginn 100g vorhanden sind, wie viel bleibt nach 15 Jahren übrig?

    $T_{1/2} = 5$ Jahre, $c = 100$g, $a = \frac{1}{2}$

    Nach 15 Jahren sind drei Halbwertszeiten vergangen:

    $f(15) = 100 \cdot \left(\frac{1}{2}\right)^3 = 100 \cdot \frac{1}{8} = 12.5$g

Aufgabe:

...folgt :-)

## Verdopplungszeit

Bei einem exponentiellen Wachstum wird die Verdopplungszeit als die Zeit definiert, in der sich die Menge
eines Stoffes verdoppelt hat. Für einen Wachstumsprozess mit der Funktion

$f(t) = c \cdot a^t$

gilt:

$T_{2} = \frac{\log(2)}{\log(a)}$

wobei $T_{2}$ die Verdopplungszeit, $c$ die Anfangsmenge und $a$ der Wachstumsfaktor ist.

Die Verdopplungszeit ist also unabhängig von der Anfangsmenge $c$ und hängt nur vom Wachstumsfaktor $a$ ab.

??? tip "Beweis"

    $f(t) = c \cdot a^t$

    $f(T_{2}) = c \cdot a^{T_{2}} = 2c$

    $\Rightarrow a^{T_{2}} = 2$

    $\Rightarrow log(a^{T_{2}}) = log(2)$

    $\Rightarrow T_{2} \cdot log(a) = log(2)$

    $\Rightarrow T_{2} = \frac{\log(2)}{\log(a)}$

??? example "Beispiel"

    Ein Bakterium verdoppelt sich alle 3 Stunden. Wenn zu Beginn 100 Bakterien vorhanden sind, wie viele sind nach 9 Stunden vorhanden?

    $T_{2} = 3$ Stunden, $c = 100$, $a = 2$

    Nach 9 Stunden sind drei Verdopplungszeiten vergangen:

    $f(9) = 100 \cdot 2^3 = 100 \cdot 8 = 800$ Bakterien

Aufgabe:

Wir legen 8000€ zu einem Jahreszins von 5% an. Wie lange dauert es, bis sich das Geld verdoppelt hat?

$k(t) = 8000 \cdot 1,05^t$

$k(T_{2}) = 8000 \cdot 1,05^{T_2} = 2 \cdot 8000$

$\Rightarrow 1,05^{T_{2}} = 2$

$\Rightarrow \log(1,05^{T_{2}}) = \log(2)$

$\Rightarrow T_{2} \cdot \log(1,05) = \log(2)$

$T_{2} = \frac{\log(2)}{\log(1,05)} = 14,2$

