# Nicht eindeutig lösbare LGS

## ⭐ Wann hat ein lineares Gleichungssystem unendlich viele Lösungen?

Ein LGS hat **unendlich viele Lösungen**, wenn:

1.  **mindestens eine Gleichung keine neue Information liefert**,  
    also eine Linearkombination anderer Gleichungen ist (→ *redundant*).

2.  Die verbleibenden Gleichungen **nicht widersprüchlich** sind.

3.  Der Rang der Koeffizientenmatrix **kleiner** ist als die Anzahl der Variablen.

Das bedeutet geometrisch:

*   In 3 Variablen sind Gleichungen **Ebenen**.
*   Unendlich viele Lösungen entstehen, wenn die Ebenen sich **in einer gemeinsamen Geraden schneiden**.


### 📘 Beispiel mit drei Gleichungen

$$
\begin{cases}
x + y + z = 3 \\
2x + 3y + z = 6 \\
3x + 4y + 2z = 9
\end{cases}
$$

### 🔎 Kurze Untersuchung

Wir verwenden leichte Zeilenumformungen.

#### 1. Z₂ – 2·Z₁

$2x + 3y + z - (2x + 2y + 2z) = 6 - 6$

Ergibt:

$Z_2' = (0,\; 1,\; -1 \;|\; 0)$

#### 2. Z₃ – 3·Z₁

$3x + 4y + 2z - (3x + 3y + 3z) = 9 - 9$

Ergibt:

$Z_3' = (0,\; 1,\; -1\;|\; 0)$

→ Zeile 2 und Zeile 3 sind **identisch** → eine Gleichung ist redundant.


### 🧮 Ergebnis nach Gauß:

$$
\begin{aligned}
x + y + z &= 3 \\
y - z &= 0 \\
\text{(keine neue Gleichung)}
\end{aligned}
$$

Zweite Gleichung liefert:

$y = z$

In die erste Gleichung einsetzen:

$x + z + z = 3$

$x = 3 - 2z$

### 🎉 Lösungsmenge (mit Parameter $t$)

$$
\boxed{
(x, y, z) = (3 - 2t,\; t,\; t), \quad t \in \mathbb{R}
}
$$

Das ist die **Parameterform einer Geraden** im Raum.

---

## Geometrische Interpretation (Beispiel Buch S. 21 Aufgabe 1a)

### 🟦 1. Jede Gleichung beschreibt eine Ebene im dreidimensionalen Raum

Das System lautet:

$$
\begin{cases}
2x+2y+2z=6 \\
2x+y-z=2 \\
4x+3y+z=8
\end{cases}
$$

Jede Gleichung ist eine **Lineare Gleichung in drei Variablen** → also eine **Ebene** im $\mathbb{R}^3$.

Wir haben also **drei Ebenen**.

### 🟩 2. Was bedeutet die Nullzeile beim Gauß-Verfahren?

Wir haben eine Nullzeile erhalten:

$$
(0\;0\;0\;|\;0)
$$

Sie bedeutet:

*   Eine Gleichung ist **überflüssig**.
*   Die dritte Ebene bringt **keine neue Bedingung** mit.
*   Die dritte Ebene ist **eine Kombination der beiden anderen**.  
    (Sie liegt also **in der gleichen Schnittgeometrie**.)

👉 **Geometrisch:**  
Alle drei Ebenen schneiden sich **nicht in einem Punkt**, aber sie sind auch **nicht parallel** →  
Sie treffen sich **entlang einer gemeinsamen Schnittgeraden**.

### 🟧 3. Zwei Ebenen schneiden sich in einer Geraden

Nimm nur die ersten beiden Ebenen:

*   Ebene $$E_1: \;2x+2y+2z = 6$$
*   Ebene $$E_2: \;2x+y-z = 2$$

Diese beiden Ebenen haben:

*   verschiedene Normalenvektoren
    $$
    n_1 = (2,2,2),\qquad n_2 = (2,1,-1)
    $$

Da die Normalen **nicht parallel** sind → die Ebenen schneiden sich entlang einer **Geraden**.

### 🟪 4. Die dritte Ebene enthält dieselbe Schnittgerade

Wir haben beim Gauß-Verfahren gesehen:

$$
Z_3 = Z_2
$$

Das heißt:

$$
4x+3y+z = 8
$$

ist eigentlich nur eine Kombination der anderen beiden Gleichungen.

👉 **Geometrisch:**  
Die dritte Ebene schneidet die ersten beiden **in der gleichen Geraden**.

Also gibt es **nur eine einzige Schnittgerade**, die alle drei Ebenen gemeinsam besitzen.

### 🔷 5. Die Lösungsmenge ist genau diese Schnittgerade

Du hast die Lösung als Parameterform:

$$
\begin{aligned}
x &= -1 + 2t \\
y &= 4 - 3t \\
z &= t
\end{aligned}
$$

Das ist die **Parameterdarstellung einer Geraden**:

$$
\vec{X}(t)
=
\begin{pmatrix}
-1 \\ 4 \\ 0
\end{pmatrix}
+
t \cdot
\begin{pmatrix}
2 \\ -3 \\ 1
\end{pmatrix}
$$

$\begin{pmatrix}-1\\4\\0\end{pmatrix}$ ist ein **Punkt auf der Geraden**

$\begin{pmatrix}2\\-3\\1\end{pmatrix}$ ist der **Richtungsvektor**, kommt also von der freien Variable

### 🏁 Geometrische Zusammenfassung

*   Jede Gleichung beschreibt eine **Ebene** im Raum.
*   Die drei Ebenen sind **nicht parallel**.
*   Keine zwei Ebenen fallen vollkommen zusammen.
*   Aber eine Ebene ist **keine neue Information** → die dritte ist eine Linearkombination der anderen.
*   Damit treffen sich die drei Ebenen **in derselben Schnittgeraden**.
*   Diese Gerade ist genau die **Lösungsmenge** des Gleichungssystems.

👉 Das Gleichungssystem ist **unendlich lösbar**, und zwar entlang dieser einen Geraden.


