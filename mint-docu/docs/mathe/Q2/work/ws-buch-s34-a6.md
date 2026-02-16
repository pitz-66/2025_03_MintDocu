# Buch Seite 34, Aufgabe 6: Investitionsproblem mit drei Anlageformen

# **1. Variablen definieren**

Wir suchen die Investitionsbeträge:

*   $$x$$ = Betrag in **Schatzbriefen** (3 %)
*   $$y$$ = Betrag in **Immobilienfonds** (5 %)
*   $$z$$ = Betrag in **Aktien** (8 %)

Gegeben ist:

$$
z = 2x
$$

***

# **2. Informationen in Gleichungen umwandeln**

### **(1) Gesamtbetrag**

$$
x + y + z = 30000
$$

### **(2) Jahresgewinn = 1820 €**

$$
0{,}03x + 0{,}05y + 0{,}08z = 1820
$$

### **(3) Aktien = doppelt so viel wie Schatzbriefe**

$$
z = 2x
$$

Damit ist unser Gleichungssystem:

$$
\begin{cases}
x + y + z = 30000 \\
0{,}03x + 0{,}05y + 0{,}08z = 1820 \\
z - 2x = 0
\end{cases}
$$

***

# **3. Gauß-Verfahren**

Wir ersetzen $$z$$ durch $$2x$$ in den ersten beiden Gleichungen.

## **Gleichung 1**

$$
x + y + 2x = 30000
$$

$$
3x + y = 30000 \quad (I)
$$

## **Gleichung 2**

$$
0{,}03x + 0{,}05y + 0{,}08(2x) = 1820
$$

$$
0{,}03x + 0{,}05y + 0{,}16x = 1820
$$

$$
0{,}19x + 0{,}05y = 1820 \quad (II)
$$

***

# **4. Gleichungssystem in Matrixform**

$$
\left(
\begin{array}{cc|c}
3 & 1 & 30000 \\
0{,}19 & 0{,}05 & 1820
\end{array}
\right)
$$

***

# **5. Gauß-Schritte**

### **Schritt 1: Zeile 2 so ändern, dass x eliminiert wird**

Wir bilden:

$$
Z_2 := Z_2 - \frac{0{,}19}{3} \cdot Z_1
$$

Berechnung des Faktors:

$$
\frac{0,19}{3} = 0{,}063333\ldots
$$

### Neue zweite Zeile:

*   x-Koeffizient:  
    $$0,19 - 0,063333\cdot 3 = 0$$

*   y-Koeffizient:  
    $$0,05 - 0,063333 = -0,013333$$

*   rechter Wert:  
    $$1820 - 0,063333\cdot 30000 = 1820 - 1900 = -80$$

Matrix:

$$
\left(
\begin{array}{cc|c}
3 & 1 & 30000 \\
0 & -0{,}013333 & -80
\end{array}
\right)
$$

***

### **Schritt 2: Zweite Zeile normieren**

$$
Z_2 := \frac{Z_2}{-0{,}013333}
$$

$$
0,\ 1,\ 6000
$$

Also:

$$
y = 6000
$$

***

### **Schritt 3: Erste Zeile berechnen**

$$
3x + y = 30000
$$

$$
3x + 6000 = 30000
$$

$$
3x = 24000
$$

$$
x = 8000
$$

***

### **Schritt 4: z aus Beziehung z = 2x**

$$
z = 2x = 2 \cdot 8000 = 16000
$$

***

# ✅ **Endergebnis**

Nikolai hat investiert:

| Anlageform                | Betrag       |
| ------------------------- | ------------ |
| **Schatzbriefe (3 %)**    | **8.000 €**  |
| **Immobilienfonds (5 %)** | **6.000 €**  |
| **Aktien (8 %)**          | **16.000 €** |

***

# **Antwort auf die Frage:**

### 👉 **Nikolai hat 16.000 € in Aktien investiert.**
