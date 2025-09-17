# Was ist Objektorientierte Programmierung (OOP)?

Objektorientierte Programmierung (OOP) ist ein Programmierparadigma, das auf dem Konzept von „Objekten“ basiert – also Einheiten, die Daten (Attribute) und Verhalten (Methoden) kombinieren. Hier sind die Antworten auf deine Fragen im Detail:

---

### **1. Unterschied zwischen prozeduraler und objektorientierter Programmierung**

| **Prozedural** | **Objektorientiert** |
|----------------|----------------------|
| Programm wird als Abfolge von Prozeduren/Funktionen geschrieben | Programm besteht aus Objekten, die miteinander interagieren |
| Daten und Funktionen sind getrennt | Daten und Funktionen sind in Klassen/Objekten vereint |
| Fokus liegt auf dem „Wie“ (Ablauf) | Fokus liegt auf dem „Was“ (Struktur und Verhalten von Objekten) |
| Beispiel: C, Pascal | Beispiel: Java, C++, Python (OOP-Stil) |

---

### **2. Drei Vorteile des objektorientierten Ansatzes**

1. **Wiederverwendbarkeit**: Einmal erstellte Klassen können in anderen Programmen oder Projekten wiederverwendet werden.
2. **Wartbarkeit**: Durch die klare Strukturierung in Objekte ist der Code leichter zu verstehen und zu pflegen.
3. **Erweiterbarkeit**: Neue Funktionen können durch Vererbung und Polymorphie einfach hinzugefügt werden, ohne bestehenden Code stark zu verändern.

---

### **3. Zwei Anwendungsbeispiele der OOP**

- **Grafische Benutzeroberflächen (GUIs)**: Jedes Element (Button, Fenster, Textfeld) ist ein Objekt mit eigenen Eigenschaften und Methoden.
- **Simulationen**: In einer Verkehrssimulation könnten Autos, Ampeln und Straßen jeweils eigene Klassen mit spezifischem Verhalten sein.

---

### **4. Objekt, Klasse, Attribut und Methode – Begriffe und Zusammenhänge**

- **Klasse**: Eine Vorlage oder ein Bauplan für Objekte. Sie definiert, welche Attribute und Methoden ein Objekt haben kann.
- **Objekt**: Eine Instanz einer Klasse. Es ist ein konkretes Exemplar mit echten Werten.
- **Attribut**: Eine Eigenschaft eines Objekts, z. B. `farbe`, `geschwindigkeit`.
- **Methode**: Eine Funktion innerhalb einer Klasse, die das Verhalten eines Objekts beschreibt, z. B. `fahre()`, `stoppe()`.

**Zusammenhang**: Die Klasse beschreibt, was ein Objekt ist und was es tun kann. Ein Objekt ist eine konkrete Ausprägung dieser Beschreibung mit individuellen Attributwerten und nutzbaren Methoden.

---

### **5. Rolle des Konstruktors**

Ein **Konstruktor** ist eine spezielle Methode, die beim Erzeugen eines Objekts automatisch aufgerufen wird. Er dient dazu, das Objekt zu initialisieren – also z. B. Anfangswerte für Attribute zu setzen.

Beispiel in Python:
```python
class Auto:
    def __init__(self, farbe):
        self.farbe = farbe
```

---

### **6. Getter und Setter – Schutz der Attribute**

- **Getter**: Methode, um den Wert eines privaten Attributs auszulesen.
- **Setter**: Methode, um den Wert eines privaten Attributs zu ändern, oft mit Validierung.

**Zweck**: Sie ermöglichen kontrollierten Zugriff auf Attribute, schützen vor unerwünschter Manipulation und erlauben z. B. Prüfungen beim Setzen von Werten.

Beispiel:
```python
class Auto:
    def __init__(self):
        self.__geschwindigkeit = 0  # privat

    def get_geschwindigkeit(self):
        return self.__geschwindigkeit

    def set_geschwindigkeit(self, wert):
        if wert >= 0:
            self.__geschwindigkeit = wert
```

---

