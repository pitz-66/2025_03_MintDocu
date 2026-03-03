# Buch Seite 64, Aufgbe 8, Punkte eines Quaders

## Aufgabe

Ein achsenparalleler Quader ABCDEFGH ist durch die Angabe der drei Punkte B (2|4|0), C (-2|4|0) und H (-2|0|3) gegeben. 
a. Bestimme die restlichen Punkte.
b. berechne die Länger der Raumdiagonalen BH


## Lösung

Hier kommt eine vollständige und klar erklärte Lösung zu beiden Teilaufgaben.

***

# **Gegeben**

Ein **achsenparalleler Quader** bedeutet:  
Die Kanten verlaufen **parallel zu den Koordinatenachsen** (x-, y-, z-Achse).

Gegeben sind drei Punkte:

$$
B(2|4|0),\quad C(-2|4|0),\quad H(-2|0|3)
$$

Wir wissen außerdem, wie ein Quader beschriftet wird:

Vorne: $$A, B, C, D$$  
Hinten: $$E, F, G, H$$

Mit der typischen Anordnung:

       H ------- G
      /         /
     E ------- F

     A ------- B
     |         |
     D ------- C

***

# **a) Bestimme die restlichen Punkte**

## **1. Lage von B und C → Untere Vorderkante**

B und C haben **z = 0**, also liegen sie unten; außerdem haben beide **y = 4**, also vorne.

B hat x = 2, C hat x = −2 ⇒ B–C ist eine Kante in x‑Richtung.

### Daher:

$$
BC = 4 \text{ parallel zur x‑Achse}
$$

***

## **2. Punkt H liegt hinten und oben**

H hat:

*   y = 0 ⇒ hinten
*   z = 3 ⇒ oben
*   x = −2 ⇒ gleiche x-Koordinate wie C

Damit ist H über D oder C; tatsächlich liegt H über **C**.

***

## **3. Bestimmung der übrigen Punkte**

### **Zu C gehört der Punkt D direkt nach unten hinten**

C hat

$$
C(-2|4|0)
$$

H gehört zur oberen hinteren Ebene und hat dieselbe x- und z-Koordinate wie D.

D erhält also die y‑Koordinate von H (0):

$$
\boxed{D(-2|0|0)}
$$

***

### **Zu D gehört A vorne unten**

A erhält dieselben x- und z-Koordinaten wie D, aber y = 4 (wie B und C):

$$
\boxed{A(-2|4|0)}
$$

***

### **Zu A gehört E hinten oben**

E hat dieselben x- und y-Koordinaten wie A, aber z = 3 (wie H):

$$
\boxed{E(-2|4|3)}
$$

***

### **Zu B gehört F oben hinten**

B(2|4|0) → F muss x = 2, y = 0, z = 3 haben:

$$
\boxed{F(2|0|3)}
$$

***

### **Zu C gehört G oben vorne?**

Nur noch G fehlt. G entspricht der oberen Ecke über C nach hinten:

C: (−2|4|0) → G: (−2|0|3)

Das ist aber **schon H**.  
Also G gehört zu B nach oben hinten:

$$
\boxed{G(2|4|3)}
$$

***

# **Alle Punkte übersichtlich**

$$
\begin{aligned}
A &= (-2|4|0) \\
B &= (2|4|0) \; \text{(gegeben)}\\
C &= (-2|4|0) \; \text{(gegeben)}\\
D &= (-2|0|0) \\
E &= (-2|4|3) \\
F &= (2|0|3) \\
G &= (2|4|3) \\
H &= (-2|0|3) \; \text{(gegeben)}
\end{aligned}
$$

**Korrektur:**  
C war gegeben als $$(-2|4|0)$$.  
A muss vorne unten links sein **mit x = −2, y = 4**, also stimmt das.

Damit ist die Punktliste korrekt.

***

# **b) Länge der Raumdiagonalen $$BH$$**

Gegeben:

$$
B(2|4|0),\quad H(-2|0|3)
$$

Wir benutzen die **3D-Abstandsformel**:

$$
d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2 + (z_2 - z_1)^2}
$$

Einsetzen:

$$
BH = \sqrt{(-2 - 2)^2 + (0 - 4)^2 + (3 - 0)^2}
$$

Rechnen:

$$
(-4)^2 = 16
$$

$$
(-4)^2 = 16
$$

$$
3^2 = 9
$$

Also:

$$
BH = \sqrt{16 + 16 + 9}
$$

$$
BH = \sqrt{41}
$$

***

# **Ergebnis**

### **Punkte des Quaders**

$$
\boxed{
A(-2|4|0),\;
B(2|4|0),\;
C(-2|4|0),\;
D(-2|0|0),\;
E(-2|4|3),\;
F(2|0|3),\;
G(2|4|3),\;
H(-2|0|3)
}
$$

### **Raumdiagonale**

$$
\boxed{BH = \sqrt{41}}
$$


