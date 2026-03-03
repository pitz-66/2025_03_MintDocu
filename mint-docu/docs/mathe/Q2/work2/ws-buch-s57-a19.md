# Buch Seite 57, Aufgbe 19, Rechtwinklige Dreiecke

## Aufgabe

Untersuche ob die Dreiecke
a) A(1|1|2), B(3|1|0), C(2|2|3)
b) A(6|2|8), B(2|6|8), C(3|6|3)
rechtwinklig sind.

## Lösung

Um festzustellen, ob ein Dreieck **rechtwinklig** ist, überprüft man, ob **zwei Seiten zueinander orthogonal** sind.  
Im Raum bedeutet das:

$$
\vec{u} \cdot \vec{v} = 0
$$

Wenn das Skalarprodukt zweier Seitenvektoren 0 ist, steht ein rechter Winkel zwischen ihnen.

***

# **a) Dreieck mit A(1|1|2), B(3|1|0), C(2|2|3)**

## **1. Seitenvektoren bilden**

$$
\vec{AB} = B - A = (3-1,\;1-1,\;0-2) = (2,0,-2)
$$

$$
\vec{AC} = C - A = (2-1,\;2-1,\;3-2) = (1,1,1)
$$

$$
\vec{BC} = C - B = (2-3,\;2-1,\;3-0) = (-1,1,3)
$$

***

## **2. Skalarprodukte prüfen**

### **AB · AC**

$$
(2,0,-2)\cdot(1,1,1) = 2\cdot1 + 0\cdot1 + (-2)\cdot1 = 2 - 2 = 0
$$

👉 **AB ⟂ AC → rechter Winkel bei A**

***

## **Ergebnis (a)**

$$
\boxed{\text{Das Dreieck ist rechtwinklig (rechter Winkel in A).}}
$$

***

# **b) Dreieck mit A(6|2|8), B(2|6|8), C(3|6|3)**

## **1. Seitenvektoren bilden**

$$
\vec{AB} = (2-6,\;6-2,\;8-8) = (-4,4,0)
$$

$$
\vec{AC} = (3-6,\;6-2,\;3-8) = (-3,4,-5)
$$

$$
\vec{BC} = (3-2,\;6-6,\;3-8) = (1,0,-5)
$$

***

## **2. Skalarprodukte prüfen**

### **AB · AC**

$$
(-4,4,0)\cdot(-3,4,-5) = 12 + 16 + 0 = 28 \neq 0
$$

### **AB · BC**

$$
(-4,4,0)\cdot(1,0,-5) = -4 + 0 + 0 = -4 \neq 0
$$

### **AC · BC**

$$
(-3,4,-5)\cdot(1,0,-5) = -3 + 0 + 25 = 22 \neq 0
$$

Keines der Skalarprodukte ist 0.

***

## **Ergebnis (b)**

$$
\boxed{\text{Das Dreieck ist nicht rechtwinklig.}}
$$

***

# **🔎 Zusammenfassung**

| Dreieck | Rechtwinklig? | Ort des rechten Winkels |
| ------- | ------------- | ----------------------- |
| a)      | ✅ Ja          | in A                    |
| b)      | ❌ Nein        | –                       |

## Alternative Lösung über Satz des Pythagoras

Gerne – wir bestimmen diesmal **nicht** über das Skalarprodukt, sondern **über die Kantenlängen** und wenden anschließend den  
👉 **Umkehrsatz des Pythagoras**  
an:

> Ein Dreieck ist rechtwinklig, wenn gilt:  
> Für drei Seitenlängen $$a \le b \le c$$ ist
>
> $$
> $$

c^2 = a^2 + b^2.
]

***

# **a) A(1|1|2), B(3|1|0), C(2|2|3)**

## **1. Seitenlängen berechnen**

Wir verwenden die 3D‑Abstandsformel:

$$
AB = \sqrt{(3-1)^2+(1-1)^2+(0-2)^2}
     = \sqrt{4+0+4}
     = \sqrt{8}
$$

$$
AC = \sqrt{(2-1)^2+(2-1)^2+(3-2)^2}
     = \sqrt{1+1+1}
     = \sqrt{3}
$$

$$
BC = \sqrt{(2-3)^2+(2-1)^2+(3-0)^2}
     = \sqrt{1+1+9}
     = \sqrt{11}
$$

Damit:

$$
AB = \sqrt{8},\quad AC = \sqrt{3},\quad BC = \sqrt{11}
$$

Sortieren nach Größe:

$$
AC < AB < BC
$$

Also ist $$BC$$ die **längste Seite** (= mögliche Hypotenuse).

***

## **2. Pythagoras prüfen**

$$
AB^2 + AC^2 = 8 + 3 = 11
$$

$$
BC^2 = 11
$$

💡 Gleichheit erfüllt:

$$
AB^2 + AC^2 = BC^2
$$

***

## ✅ **Ergebnis (a)**

$$
\boxed{\text{Das Dreieck ist rechtwinklig (rechter Winkel bei A).}}
$$

***

# **b) A(6|2|8), B(2|6|8), C(3|6|3)**

## **1. Seitenlängen berechnen**

$$
AB = \sqrt{(2-6)^2+(6-2)^2+(8-8)^2}
     = \sqrt{16+16+0}
     = \sqrt{32}
$$

$$
AC = \sqrt{(3-6)^2+(6-2)^2+(3-8)^2}
     = \sqrt{9+16+25}
     = \sqrt{50}
$$

$$
BC = \sqrt{(3-2)^2+(6-6)^2+(3-8)^2}
     = \sqrt{1+0+25}
     = \sqrt{26}
$$

Sortieren:

$$
BC < AB < AC
$$

Also ist $$AC$$ die längste Seite (mögliche Hypotenuse).

***

## **2. Pythagoras prüfen**

$$
AB^2 + BC^2 = 32 + 26 = 58
$$

$$
AC^2 = 50
$$

Die beiden Werte sind **nicht gleich**:

$$
58 \ne 50
$$

***

## ❌ **Ergebnis (b)**

$$
\boxed{\text{Das Dreieck ist nicht rechtwinklig.}}
$$

***

# 🎉 **Endergebnis**

| Dreieck | Rechtwinklig? | Begründung                                    |
| ------- | ------------- | --------------------------------------------- |
| **a)**  | ✅ Ja          | $$AB^2 + AC^2 = BC^2$$                        |
| **b)**  | ❌ Nein        | Keine Kombination erfüllt $$a^2 + b^2 = c^2$$ |



