# Nicht lösbare lineare Gleichungssysteme

## 🔸 Warum können 3 Gleichungen in 3 Variablen unlösbar sein?

Ein lineares Gleichungssystem mit drei Gleichungen beschreibt **drei Ebenen im dreidimensionalen Raum**.  
Ein System ist **unlösbar**, wenn diese Ebenen **keinen gemeinsamen Punkt** besitzen.

Das kann auf verschiedene Arten passieren:

### 1. Die Ebenen schneiden sich nicht alle gemeinsam

#### ➤ Zwei Ebenen schneiden sich in einer Geraden,

aber die dritte Ebene **verfehlt** diese Gerade.

Dies ist der häufigste Fall von Unlösbarkeit.

**Geometrisch:**  
Alle Ebenen schneiden sich paarweise, aber **kein Punkt** liegt in allen drei Ebenen gleichzeitig.

### 2. Zwei Ebenen sind parallel, die dritte schneidet sie nicht

Wenn zwei Ebenen parallel sind, gibt es **keinen Schnittpunkt** zwischen ihnen.  
Egal wie die dritte Ebene liegt – ein gemeinsamer Punkt aller drei kann nicht existieren.

### 3. Drei Ebenen sind alle parallel (extrem seltener Fall)

Wenn alle Normalenvektoren parallel sind, aber die Ebenen auf unterschiedlichen Höhen liegen, schneiden sie sich überhaupt nicht.

➡️ Dann ist das System ebenfalls **unlösbar**.

### 🔥 Woran erkennt man Unlösbarkeit rechnerisch?

Beim Gauß‑Verfahren erscheint dann eine Zeile der Form:

$0x + 0y + 0z = c \quad \text{mit } c \neq 0$

also z.B.:

$0 = -6$

Das ist ein **Widerspruch** → keine Lösung.

### 📌 Kurz: Warum unlösbar?

Weil die drei Ebenen **geometrisch keine gemeinsame Schnittmenge** besitzen.

Sie treffen sich entweder:

*   in **paarweisen Geraden**, aber nicht gemeinsam, oder
*   zwei sind parallel, oder
*   alle sind parallel.

In jedem Fall gibt es **keinen einzigen Punkt**, der in allen drei Ebenen liegt.

## Geometrische Interpretation (Beispiel Buch S. 21 Aufgabe 1b)

### 🔢 Ausgangspunkt: Das Gleichungssystem

$$
\begin{cases}
3x + 5y - 2z = 10 \\
2x + 8y - 5z = 6 \\
4x + 2y + z = 8
\end{cases}
$$

Wie immer gilt:  
**Jede Gleichung in drei Variablen beschreibt eine Ebene im dreidimensionalen Raum.**

Wir haben also **drei Ebenen**:

*   $E_1: 3x + 5y - 2z = 10$
*   $E_2: 2x + 8y - 5z = 6$
*   $E_3: 4x + 2y + z = 8$

### 🟦 Schritt 1: Was zeigte die Rechnung?

Beim Gauß‑Algorithmus entstand die letzte Zeile:

$$
0x + 0y + 0z = -6
\quad\Rightarrow\quad 0 = -6
$$

Das ist **unmöglich** → das System ist **widersprüchlich**.

➡️ Geometrisch heißt das:  
Die drei Ebenen besitzen **keinen gemeinsamen Schnittpunkt** und auch **keine gemeinsame Schnittgerade**.

### 🟧 Schritt 2: Was passiert geometrisch mit Ebenen?

In $\mathbb{R}^3$ können drei Ebenen:

1.  **Einen gemeinsamen Punkt besitzen** → eindeutige Lösung
2.  **Eine gemeinsame Gerade besitzen** → unendlich viele Lösungen
3.  **Sich paarweise schneiden, aber nicht alle drei zusammen** → keine Lösung
4.  **Zwei Ebenen parallel sein bzw. eine Ebene parallel zu der Schnittgeraden der anderen beiden** → keine Lösung
5.  **Sich in einem „Dreikanten“-Muster schneiden (je zwei schneiden sich, aber kein gemeinsamer Schnittpunkt)** → keine Lösung

### 🔴 Schritt 3: Was bedeutet die widersprüchliche Zeile konkret?

Dass aus zwei Ebenen z.B. folgt:

$E_3: 4x + 2y + z = 8$

und durch Kombination von $E_1$ und $E_2$ würde (theoretisch) eine Gleichung entstehen, die etwas völlig anderes fordert, z.B.:

$4x + 2y + z = 14$

Das heißt:

*   Die Lage von Ebene 3 stimmt **nicht** mit der Lage überein, die sich aus den ersten beiden Ebenen ergeben müsste.

➡️ **E₃ liegt auf der „falschen Position“**, sodass sie die gemeinsame Schnittlinie (oder Schnittpunkt) von $E_1$ und $E_2$ **verfehlt**.

### 🟩 Schritt 4: Was bedeutet das räumlich?

#### 🔍 Ebene 1 und Ebene 2 schneiden sich in einer Geraden.

Denn ihre Normalenvektoren sind nicht parallel.

Die beiden Ebenen bilden also eine Schnittgerade:

$g = E_1 \cap E_2$

#### 🔍 Ebene 3 schneidet diese Gerade jedoch NICHT.

Das heißt:

*   Ebene $E_3$ liegt „versetzt“,
*   schneidet aber trotzdem jede einzelne der beiden anderen Ebenen irgendwo,
*   **aber eben nicht genau auf deren gemeinsamer Schnittgerade**.

Das ist die typische „Dreikanten“-Situation:

#### ➤ Die drei Ebenen schneiden sich paarweise,

aber **kein Punkt liegt in allen drei Ebenen gleichzeitig**.

## 🎨 Bildlich kannst du dir das vorstellen als:

*   Zwei Ebenen bilden eine schräg stehende „Buchseite" → sie haben eine Schnittgerade.
*   Die dritte Ebene ist wie eine weitere Seite, die aber **nicht genau** durch die Schnittlinie geht, sondern etwas daneben liegt.
*   Dadurch entsteht **kein gemeinsamer Punkt**.

## 🟠 Schritt 5: Zusammenfassung

Das Gleichungssystem ist **nicht lösbar**, weil:

*   Ebenen $E_1$ und $E_2$ schneiden sich in einer Geraden.
*   Ebene $E_3$ ist jedoch **parallel zu dieser Schnittgeraden**, aber nicht in ihr enthalten.
*   Damit entsteht **keine gemeinsame Schnittmenge** aller drei Ebenen.

➡️ **Ergebnis:**

$$
\boxed{L = \varnothing}
$$
