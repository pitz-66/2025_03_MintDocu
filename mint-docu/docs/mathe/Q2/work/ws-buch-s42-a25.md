# Buch Seite 42, Aufgabe 25: Mischungsproblem mit drei Sorten

# **1. Variablen definieren**

Wir suchen die Mengen der drei Sorten:

*   $$x$$ = kg Sorte A
*   $$y$$ = kg Sorte B
*   $$z$$ = kg Sorte C

***

# **2. Mischungsbedingungen**

### **Holzanteile der Sorten**

| Sorte | Eiche | Birke |
| ----- | ----- | ----- |
| A     | 20%   | 60%   |
| B     | 30%   | 40%   |
| C     | 70%   | 10%   |

### **Bestellung des Kunden**

*   **Gesamtmenge:** 1000 kg
*   **Eiche:** 400 kg
*   **Birke:** 350 kg

***

# **3. Gleichungssystem aufstellen**

## **Gesamtmasse**

$$
x + y + z = 1000
$$

## **Eichenholz**

$$
0{,}20x + 0{,}30y + 0{,}70z = 400
$$

## **Birkenholz**

$$
0{,}60x + 0{,}40y + 0{,}10z = 350
$$

Damit haben wir das lineare Gleichungssystem:

$$
\begin{cases}
x + y + z = 1000 \\
0{,}20x + 0{,}30y + 0{,}70z = 400 \\
0{,}60x + 0{,}40y + 0{,}10z = 350
\end{cases}
$$

***

# **4. Gauß-Verfahren**

Wir beginnen mit der erweiterten Matrix:

$$
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 1000 \\
0{,}2 & 0{,}3 & 0{,}7 & 400 \\
0{,}6 & 0{,}4 & 0{,}1 & 350
\end{array}
\right)
$$

***

## **Schritt 1: Zeile 2 und Zeile 3 von Zeile 1 befreien**

### Z2 := Z2 – 0,2·Z1

*   $$0,3 - 0,2 = 0,1$$
*   $$0,7 - 0,2 = 0,5$$
*   $$400 - 200 = 200$$

Ergebnis:

$$
(0,\ 0{,}1,\ 0{,}5\ |\ 200)
$$

### Z3 := Z3 – 0,6·Z1

*   $$0,4 - 0,6 = -0,2$$
*   $$0,1 - 0,6 = -0,5$$
*   $$350 - 600 = -250$$

Ergebnis:

$$
(0,\ -0{,}2,\ -0{,}5\ |\ -250)
$$

Neue Matrix:

$$
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 1000 \\
0 & 0{,}1 & 0{,}5 & 200 \\
0 & -0{,}2 & -0{,}5 & -250
\end{array}
\right)
$$

***

## **Schritt 2: Z3 von Z2 befreien**

Wir bilden Z3 := Z3 + 2·Z2

In Z2:

*   $$0{,}1 \cdot 2 = 0{,}2$$
*   $$0{,}5 \cdot 2 = 1{,}0$$
*   $$200 \cdot 2 = 400$$

Rechnung:

*   $$-0{,}2 + 0{,}2 = 0$$
*   $$-0{,}5 + 1{,}0 = 0{,}5$$
*   $$-250 + 400 = 150$$

Neue Z3:

$$
(0,\ 0,\ 0{,}5\ |\ 150)
$$

***

## **Schritt 3: Z3 normalisieren**

Z3 := Z3 / 0,5

$$
(0,\ 0,\ 1\ |\ 300)
$$

Also:

$$
z = 300
$$

***

## **Schritt 4: Z2 berechnen**

Z2:

$$
0{,}1y + 0{,}5z = 200
$$

Einsetzen von $$z = 300$$:

$$
0{,}1y + 150 = 200
$$

$$
0{,}1y = 50
$$

$$
y = 500
$$

***

## **Schritt 5: Z1 berechnen**

$$
x + y + z = 1000
$$

$$
x + 500 + 300 = 1000
$$

$$
x = 200
$$

***

# ✅ **Endergebnis**

Der Händler muss mischen:

| Sorte | Menge      |
| ----- | ---------- |
| **A** | **200 kg** |
| **B** | **500 kg** |
| **C** | **300 kg** |


