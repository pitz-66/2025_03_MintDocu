# Buch Seite 46

### Aufgabe 1

Bestimme die Stammfunktion der folgenden Funktionen.

#### a) $f(x) = x^4$

??? success "Lösung"
    
    Potenzregel
    
    $F(x) = \frac{1}{5}x^5 + C$

#### b) $f(x) = 2x^3-x+3$

??? success "Lösung"
    
    Summenregel, Faktor bleibt, Potenzregel
    
    $F(x) = 2\frac{1}{4}x^4 - \frac{1}{2}x^2 + 3x + C$

#### c) $f(x) = \frac{6}{x^2}$

??? success "Lösung"
    
    Potenz im Nenner -> Negativer Exponent im Zähler
    
    $f(x)=\frac{6}{x^2} = 6x^{-2}$
    
    Faktor bleibt, Potenzregel
    
    $F(x) = 6\cdot -x^{-1} + C = -\frac{6}{x} + C$

#### d) $f(x) = (2x+1)^3$

??? success "Lösung"
    
    Kettenregel rückwärts, Faktor 3 bleibt, Potenzregel
    
    $F(x) = \frac{1}{2} \cdot \frac{1}{4}(2x+1)^4 + C = \frac{1}{8}(2x+1)^4 + C$

#### e) $f(x) = 2e^{-x}$
??? success "Lösung"
    
    Faktor 2 bleibt, Der Faktor vor dem x (-1) ziehen wir vor die e-Funktion als Kehrwert
    
    $F(x) = 2 \cdot \frac{1}{-1} \cdot e^{-x} + C = -2e^{-x} + C$

#### f) $f(x) = 3 sin(\pi\cdot x + \pi)$

??? success "Lösung"
    
    Faktor 3 bleibt, Der Faktor vor dem x ($\pi$) wird vor die sin-Funktion als Kehrwert gezogen
    
    $F(x) = 3 \cdot \frac{1}{\pi} \cdot -cos(\pi\cdot x + \pi) + C = -\frac{3}{\pi}cos(\pi\cdot x + \pi) + C$

#### g) $f(x) = 4e^{2x+\frac{1}{2}}$

??? success "Lösung"
    
    Faktor 4 bleibt, Der Faktor vor dem x (2) ziehen wir vor die e-Funktion als Kehrwert
    
    $F(x) = 4 \cdot \frac{1}{2} \cdot e^{2x+\frac{1}{2}} + C = 2e^{2x+\frac{1}{2}} + C$

### Aufgabe 5

#### b)
Berechnen Sie den Inhalt der Fläche zwischen den beiden Nullstellen der Funktion

$f(x)=x^2-6x+8$

??? success "Lösung"
    
    Nullstellen berechnen:
    
    $0 = x^2-6x+8$
    
    $0 = (x-2)(x-4)$
    
    $x_1 = 2, x_2 = 4$
    
    Stammfunktion bestimmen:
    
    $F(x) = \frac{1}{3}x^3 - 3x^2 + 8x + C$
    
    Flächeninhalt berechnen:
    
    $A = F(4) - F(2)$
    
    $A = \left[\frac{1}{3} \cdot 4^3 - 3 \cdot 4^2 + 8 \cdot 4\right] - \left[\frac{1}{3} \cdot 2^3 - 3 \cdot 2^2 + 8 \cdot 2\right]$
    
    $A = \left[\frac{64}{3} - 48 + 32\right] - \left[\frac{8}{3} - 12 + 16\right]$
    
    $A = \left[\frac{64}{3} - 16\right] - \left[\frac{8}{3} + 4\right]$
    
    $A = \frac{64}{3} - \frac{48}{3} - \frac{8}{3} - \frac{12}{3}$
    
    $A = \frac{64 - 48 - 8 - 12}{3}$
    
    $A = \frac{-4}{3}$
    
    Da der Flächeninhalt positiv sein muss, nehmen wir den Betrag:
    
    $A = \frac{4}{3}$


