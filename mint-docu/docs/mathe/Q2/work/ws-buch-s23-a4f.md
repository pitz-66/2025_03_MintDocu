# Buch Seite 23, Aufgabe 4f: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

## 🔢 Gegebenes Gleichungssystem

$$
\begin{cases}
3x - 4y + z = 5 \\
2x - y - z = 0 \\
4x - 2y - 2z = 12
\end{cases}
$$

## ➤ Schritt 1: Erstelle die erweiterte Matrix

$$
\left(
\begin{array}{ccc|c}
3 & -4 & 1 & 5 \\
2 & -1 & -1 & 0 \\
4 & -2 & -2 & 12
\end{array}
\right)
$$

## ➤ Schritt 2: Eliminiere $$x$$ aus Zeile 3

Wir nutzen Zeile 2 als Pivot:

Zeile 2 × 2:

$$
(2x - y - z = 0)\cdot 2 \quad\Rightarrow\quad 4x - 2y - 2z = 0
$$

Vergleich mit Zeile 3:

$$
Z_3: \quad 4x - 2y - 2z = 12
$$

Nun:

$$
Z_3 - 2Z_2 \Rightarrow (4x - 2y - 2z) - (4x - 2y - 2z) = 12 - 0
$$

Dies ergibt:

$$
0 = 12
$$

## ❗ Widerspruch

Die Gleichungen **2** und **3** widersprechen sich direkt:

*   Aus Gleichung 2 folgt:
    $$
    4x - 2y - 2z = 0
    $$
*   Aus Gleichung 3 folgt:
    $$
    4x - 2y - 2z = 12
    $$

Damit ist das gesamte System **inkonsistent**.

## ✅ **Lösungsmenge**

$$
\boxed{\emptyset}
$$

Es gibt **keine Lösung** – das Gleichungssystem ist *widersprüchlich*.

