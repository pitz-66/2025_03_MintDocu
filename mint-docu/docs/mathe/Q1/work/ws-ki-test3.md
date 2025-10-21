# Testaufagabe 3


**Aufgabe:**  
Berechne die Fläche unter dem Graphen der Funktion 

$f(x) = \frac{1}{x} $ im Intervall [1, 2]

mit Hilfe der Streifenmethode (Rechteckmethode) und anschließender Grenzwertbetrachtung.

---

**Lösung:**  
1. Teile das Intervall [1, 2] in n gleich große Streifen der Breite </br>
   $\Delta x = \frac{2-1}{n} = \frac{1}{n}$

2. Die Stützstellen (rechte Riemann-Summe) sind</br>
   $x_k = 1 + k \cdot \Delta x$ für $k = 1, 2, ..., n$
3. Die Summe der Rechtecksflächen ist:
   \[
   S_n = \sum_{k=1}^{n} f(x_k) \cdot \Delta x = \sum_{k=1}^{n} \frac{1}{1 + \frac{k}{n}} \cdot \frac{1}{n}
   \]
   Schreibe \(x_k = 1 + \frac{k}{n}\), also:
   \[
   S_n = \sum_{k=1}^{n} \frac{1}{1 + \frac{k}{n}} \cdot \frac{1}{n}
   \]
4. Grenzwert für \(n \to \infty\):
   \[
   \lim_{n \to \infty} S_n = \int_{1}^{2} \frac{1}{x} dx = [\ln x]_{1}^{2} = \ln 2 - \ln 1 = \ln 2
   \]
   Also ist die gesuchte Fläche \(\ln 2\).

---

**Antwort:**  
Die Fläche unter \(f(x) = \frac{1}{x}\) von \(x=1\) bis \(x=2\) beträgt \(\ln 2\).