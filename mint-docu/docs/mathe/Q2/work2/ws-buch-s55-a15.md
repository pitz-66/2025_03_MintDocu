# Buch Seite 55, Aufgbe 15, Punkte eines Würfels

## Aufgabe
Ein achsenparalleler Würfel ABCDEFGH ist durch die Angabe der drei Punkte 
A (1|1|0)
D (1|5|0)
G (5|5|4) gegeben. 
a. Bestimme die restlichen Punkte.
b. berechne die Länge der Raumdiagonalen

## Lösung

Hier kommt eine vollständige, verständlich erklärte Lösung zu beiden Teilaufgaben.

***

# ✅ **Gegeben**

Ein **achsenparalleler Würfel** bedeutet:

*   Alle Kanten sind **gleich lang**.
*   Sie verlaufen **parallel zu den Koordinatenachsen**.
*   Punkte sind wie gewohnt beschriftet:

<!---->

       E ---- F
      /      /
     A ---- B

       H ---- G
      /      /
     D ---- C

(Es gibt verschiedene Beschriftungsvarianten; deine Daten entsprechen einer üblichen Schulbuchvariante.)

Gegeben sind drei Punkte:

$$
A(1|1|0),\quad D(1|5|0),\quad G(5|5|4)
$$

***

# ✨ Schritt 1: Kantenlängen bestimmen

Vergleiche **A → D**:

$$
A(1,1,0),\quad D(1,5,0)
$$

Nur die **y-Koordinate** ändert sich:

$$
5 - 1 = 4
$$

Damit beträgt die Würfelkante:

$$
a = 4
$$

Auch bei **z** bestätigt G:

$$
G(5,5,4) \Rightarrow z = 4 = a
$$

***

# ✨ Schritt 2: Alle Punkte bestimmen

Wir starten mit den gegebenen und ergänzen systematisch die restlichen.

***

## **Unteres Quadrat (z = 0)**

### Gegeben:

*   $$A(1|1|0)$$
*   $$D(1|5|0)$$

### Punkt B

B liegt neben A in **x‑Richtung**:

$$
B = (1+4,\;1,\;0) = (5|1|0)
$$

### Punkt C

C ist neben D in **x‑Richtung**:

$$
C = (1+4,\;5,\;0) = (5|5|0)
$$

***

## **Oberes Quadrat (z = 4)**

G ist bereits bekannt:

$$
G(5|5|4)
$$

### Punkt E über A:

$$
E = (1,\;1,\;4)
$$

### Punkt F über B:

$$
F = (5,\;1,\;4)
$$

### Punkt H über D:

$$
H = (1,\;5,\;4)
$$

***

# ✅ **Alle Würfelpunkte**

$$
\begin{aligned}
A &= (1|1|0) \\
B &= (5|1|0) \\
C &= (5|5|0) \\
D &= (1|5|0) \\
E &= (1|1|4) \\
F &= (5|1|4) \\
G &= (5|5|4) \\
H &= (1|5|4)
\end{aligned}
$$

***

# **b) Länge der Raumdiagonale**

Die Raumdiagonale eines Würfels ist z.B. $$AG$$:

$$
A(1|1|0),\quad G(5|5|4)
$$

Wir verwenden die 3D‑Abstandsformel:

$$
d = \sqrt{(x_2-x_1)^2 + (y_2-y_1)^2 + (z_2-z_1)^2}
$$

Einsetzen:

$$
AG = \sqrt{(5-1)^2 + (5-1)^2 + (4-0)^2}
$$

$$
AG = \sqrt{4^2 + 4^2 + 4^2}
$$

$$
AG = \sqrt{3\cdot 16}
$$

$$
\boxed{AG = 4\sqrt{3}}
$$

Das ist die übliche Formel für die Raumdiagonale eines Würfels:

$$
d = a\sqrt{3}
$$

***

# 🎉 **Endergebnis**

### **a) Punkte des Würfels**

$$
\boxed{
A(1|1|0),\, B(5|1|0),\, C(5|5|0),\, D(1|5|0),\,
E(1|1|4),\, F(5|1|4),\, G(5|5|4),\, H(1|5|4)
}
$$

### **b) Raumdiagonale**

$$
\boxed{4\sqrt{3}}
$$

