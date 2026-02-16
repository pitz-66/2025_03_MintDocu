# Buch Seite 42, Aufgabe 23: Rotweinmischung

# **1. Variablen definieren**

*   $$x$$ = Menge **Rotwein guter Qualität** (in Hektolitern)
*   $$y$$ = Menge **Rotwein mittlerer Qualität** (in Hektolitern)

***

# **2. Mischungsbedingungen aufstellen**

Der Winzer hat:

*   **30 hl Merlot**
*   **29 hl Cabernet Sauvignon**

## Zusammensetzungen:

| Wein              | Merlot | Cabernet |
| ----------------- | ------ | -------- |
| Gute Qualität     | 25%    | 75%      |
| Mittlere Qualität | 75%    | 25%      |

***

# **3. Gleichungssystem aufstellen**

### **Merlot-Gleichung:**

$$
0{,}25x + 0{,}75y = 30
$$

### **Cabernet-Gleichung:**

$$
0{,}75x + 0{,}25y = 29
$$

Damit lautet das lineare Gleichungssystem:

$$
\begin{cases}
0{,}25x + 0{,}75y = 30 \\
0{,}75x + 0{,}25y = 29
\end{cases}
$$

***

# **4. Gauß-Verfahren anwenden**

Schreiben als erweitertes Gleichungssystem:

$$
\left(
\begin{array}{cc|c}
0{,}25 & 0{,}75 & 30 \\
0{,}75 & 0{,}25 & 29
\end{array}
\right)
$$

### **Schritt 1: Erste Zeile × 4**

$$
\left(
\begin{array}{cc|c}
1 & 3 & 120 \\
0{,}75 & 0{,}25 & 29
\end{array}
\right)
$$

### **Schritt 2: Zweite Zeile – 0,75·(Erste Zeile)**

Berechnen:

*   $$0,75 - 0,75\cdot1 = 0$$
*   $$0,25 - 0,75\cdot3 = 0,25 - 2,25 = -2$$
*   $$29 - 0,75\cdot120 = 29 - 90 = -61$$

Ergebnis:

$$
\left(
\begin{array}{cc|c}
1 & 3 & 120 \\
0 & -2 & -61
\end{array}
\right)
$$

### **Schritt 3: Zweite Zeile durch –2 teilen**

$$
\left(
\begin{array}{cc|c}
1 & 3 & 120 \\
0 & 1 & 30,5
\end{array}
\right)
$$

### **Schritt 4: Erste Zeile bereinigen**

1.  Zeile – 3·(2. Zeile):

*   $$3 - 3\cdot1 = 0$$
*   $$120 - 3\cdot30,5 = 120 - 91,5 = 28,5$$

Ergebnis:

$$
\left(
\begin{array}{cc|c}
1 & 0 & 28,5 \\
0 & 1 & 30,5
\end{array}
\right)
$$

***

# **5. Lösung**

$$
x = 28{,}5 \quad\text{hl (gute Qualität)}
$$

$$
y = 30{,}5 \quad\text{hl (mittlere Qualität)}
$$

***

# ✅ **Endergebnis**

Der Winzer stellt her:

*   **28,5 hl Rotwein guter Qualität**
*   **30,5 hl Rotwein mittlerer Qualität**

