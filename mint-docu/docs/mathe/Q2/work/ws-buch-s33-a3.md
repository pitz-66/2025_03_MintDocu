# Buch Seite 33, Aufgabe 3

## Gegeben

David, Tina und Georg haben zusammen **160€**.

Zusatzinformationen:

*   **David hat am meisten.**
*   **David besitzt 24€ mehr als Georg.** $D = G + 24$
*   **Tina hat am wenigsten.**
*   **Tina besitzt 14€ weniger als Georg.** $T = G - 14$

Gesucht: **Ersparnis von Tina**.

## 1. Variablen einführen

*   $D$: Davids Ersparnis
*   $G$: Georgs Ersparnis
*   $T$: Tinas Ersparnis

## 2. Gleichungssystem aufstellen

### (1) Gesamtsumme:

$D + T + G = 160$

### (2) David hat 24€ mehr als Georg:

$D = G + 24$

### (3) Tina hat 14€ weniger als Georg:

$T = G - 14$

## 3. Gleichungssystem reduzieren

Setze (2) und (3) in die Summengleichung (1) ein:

$(G+24) + (G-14) + G = 160$

Ausrechnen:

$3G + 10 = 160$

$3G = 150$

$G = 50$

Jetzt rückwärts einsetzen:

#### David:

$D = G + 24 = 50 + 24 = 74$

#### Tina:

$T = G - 14 = 50 - 14 = 36$

## 4. Gauß-Algorithmus (optional)

LGS in Standardform:

$$
\begin{cases}
D - G = 24 \\
T - G = -14 \\
D + T + G = 160
\end{cases}
$$

Matrix:

$$
\begin{pmatrix}
1 & -1 & 0 & | & 24 \\
0 & -1 & 1 & | & -14 \\
1 & 1 & 1 & | & 160
\end{pmatrix}
$$

Nach Eliminationsschritten erhält man:

$$
\begin{pmatrix}
1 & -1 & 0 & | & 24 \\
0 & -1 & 1 & | & -14 \\
0 & 0 & 3 & | & 150
\end{pmatrix}
$$

Letzte Zeile:

$$
3G = 150 \Rightarrow G = 50
$$

Dann:

$$
T = G - 14 = 36
$$

$$
D = G + 24 = 74
$$

# ✅ **Endergebnis**

**Tina hat 36€**



