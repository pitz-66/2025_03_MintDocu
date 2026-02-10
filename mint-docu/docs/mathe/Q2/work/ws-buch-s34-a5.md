# Buch Seite 34, Aufgabe 5

Ein Kino verkauft drei Arten von Eintrittskarten:

*   **Vollpreis:** 9€
*   **Rentner:** 6€
*   **Studenten:** 5€

In einer Vorstellung wurden **400 Karten** verkauft und dabei **3300€** eingenommen.  
Außerdem gilt:  
👉 *Die Anzahl der Studentenkarten ist dreimal so groß wie die Anzahl der Rentnerkarten.*

**Gesucht:** Anzahl der verkauften **Vollpreiskarten**.

## 1. Variablen einführen

*   $x$: Anzahl Vollpreiskarten
*   $y$: Anzahl Rentnerkarten
*   $z$: Anzahl Studentenkarten

## 2. Gleichungen aufstellen

### (1) Gesamtanzahl Karten:

$x + y + z = 400$

### (2) Gesamteinnahmen:

$9x + 6y + 5z = 3300$

### (3) Verhältnis Studenten–Rentner:

$z = 3y$

Damit haben wir ein lineares Gleichungssystem aus drei Gleichungen.

# 3. Einsetzen von $z = 3y$

Setze in (1) und (2) ein:

### In (1):

$x + y + 3y = 400$

$x + 4y = 400$

### In (2):

$9x + 6y + 5(3y) = 3300$

$9x + 6y + 15y = 3300$

$9x + 21y = 3300$

Wir haben nun ein 2×2‑System:

$$
\begin{cases}
x + 4y = 400 \\
9x + 21y = 3300
\end{cases}
$$

## 4. Gaußscher Eliminationsalgorithmus

Schreibe die erweiterte Matrix:

$$
\begin{pmatrix}
1 & 4 & | & 400 \\
9 & 21 & | & 3300
\end{pmatrix}
$$

### Schritt 1: Eliminieren des $x$-Terms in Zeile 2

$$
Z_2 \leftarrow Z_2 - 9Z_1
$$

Berechnung:

*   $21 - 36 = -15$
*   $3300 - 3600 = -300$

Neue Matrix:

$$
\begin{pmatrix}
1 & 4 & | & 400 \\
0 & -15 & | & -300
\end{pmatrix}
$$

### Schritt 2: Auflösen nach $y$

$$
-15y = -300 \quad\Rightarrow\quad y = 20
$$

### Schritt 3: Rückeinsetzen

In $x + 4y = 400$:

$x + 4(20) = 400$

$x + 80 = 400$

$x = 320$

### Schritt 4: $z = 3y$

$z = 3 \cdot 20 = 60$

### ✅ Ergebnis

*   **Vollpreiskarten:** **320**
*   Rentnerkarten: 20
*   Studentenkarten: 60

## ✔️ Kontrolle

$$
320 + 20 + 60 = 400
$$

$$
9\cdot 320 + 6\cdot 20 + 5\cdot 60
= 2880 + 120 + 300
= 3300
$$

