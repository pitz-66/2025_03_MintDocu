# Buch Seite 21 Übung 1b: Lösbarkeit und Lösungsmenge eines LGS mit dem Gauß-Verfahren

## 🔢 Gegebenes lineares Gleichungssystem

$$
\begin{cases}
3x + 5y - 2z = 10 \\
2x + 8y - 5z = 6 \\
4x + 2y + z = 8
\end{cases}
$$

Wir benutzen das **Gauß‑Verfahren**, um zu prüfen, ob das System:

*   eine eindeutige Lösung,
*   unendlich viele Lösungen oder
*   keine Lösung

hat.

## ✅ 1. Erweiterte Matrix aufstellen

$$
\left[
\begin{array}{ccc|c}
3 & 5 & -2 & 10 \\
2 & 8 & -5 & 6 \\
4 & 2 & 1 & 8
\end{array}
\right]
$$

## ✅ 2. Erste Spalte unterhalb von Zeile 1 eliminieren

### Z₂ := Z₂ – (2/3)·Z₁

$(2,\;8,\;-5,\;6) - (2,\; \tfrac{10}{3},\;-\tfrac{4}{3},\;\tfrac{20}{3})$

Ergebnis:

$$
Z_2= \left[\begin{array}{ccc|c}
0 & \tfrac{14}{3} & -\tfrac{11}{3} & -\tfrac{2}{3}
\end{array}\right]
$$

### Z₃ := Z₃ – (4/3)·Z₁

$(4,\;2,\;1,\;8) - (4,\;\tfrac{20}{3},\;-\tfrac{8}{3},\;\tfrac{40}{3})$

Ergebnis:

$$
Z_3=\left[\begin{array}{ccc|c}
0 & -\tfrac{14}{3} & \tfrac{11}{3} & -\tfrac{16}{3}
\end{array}\right]
$$

## ✔️ Neue Matrix

$$
\left[
\begin{array}{ccc|c}
3 & 5 & -2 & 10 \\
0 & \tfrac{14}{3} & -\tfrac{11}{3} & -\tfrac{2}{3} \\
0 & -\tfrac{14}{3} & \tfrac{11}{3} & -\tfrac{16}{3}
\end{array}
\right]
$$

## ✅ 3. Zweite Spalte unterhalb von Zeile 2 eliminieren

### Z₃ := Z₃ + Z₂

$$
\left(0,\; -\tfrac{14}{3},\;\tfrac{11}{3},\; -\tfrac{16}{3}\right)
+
\left(0,\;\tfrac{14}{3},\;-\tfrac{11}{3},\; -\tfrac{2}{3}\right)
$$

Ergebnis:

$$
Z_3= \left[\begin{array}{ccc|c}
0 & 0 & 0 & -6 \\
\end{array}\right]
$$

## ❌ 4. Nullzeile mit Nicht‑Null rechts → Widerspruch

Letzte Zeile lautet:

$0x + 0y + 0z = -6$

Das bedeutet:

$0 = -6$

➡️ **Widerspruch**

➡️ Keine Lösung möglich

# 🚫 Lösbarkeit

Das Gleichungssystem ist **nicht lösbar**.

Es handelt sich um ein **inkonsistentes System**.

## 📌 Lösungsmenge

$$
\boxed{L = \varnothing}
$$

Das System besitzt **keine Lösung**.

