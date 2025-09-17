# Was ist OOP: Beispiel
Hier ist ein einfaches Beispielprogramm in **Java**, das die Konzepte **Klasse**, **Objekt**, **Attribute**, **Methoden**, **Konstruktor**, **Getter** und **Setter** demonstriert:

---

### 🚗 Beispiel: Klasse `Auto`

```java
public class Auto {
    // Attribute (Eigenschaften)
    private String farbe;
    private int geschwindigkeit;

    // Konstruktor
    public Auto(String farbe) {
        this.farbe = farbe;
        this.geschwindigkeit = 0; // Standardwert
    }

    // Getter für Farbe
    public String getFarbe() {
        return farbe;
    }

    // Setter für Farbe
    public void setFarbe(String farbe) {
        this.farbe = farbe;
    }

    // Getter für Geschwindigkeit
    public int getGeschwindigkeit() {
        return geschwindigkeit;
    }

    // Setter für Geschwindigkeit mit Validierung
    public void setGeschwindigkeit(int geschwindigkeit) {
        if (geschwindigkeit >= 0) {
            this.geschwindigkeit = geschwindigkeit;
        } else {
            System.out.println("Ungültige Geschwindigkeit!");
        }
    }

    // Methode: Auto fährt
    public void fahre() {
        System.out.println("Das Auto fährt mit " + geschwindigkeit + " km/h.");
    }

    // Methode: Auto stoppt
    public void stoppe() {
        geschwindigkeit = 0;
        System.out.println("Das Auto wurde gestoppt.");
    }
}
```

---

### 🧪 Verwendung der Klasse `Auto` in der `main`-Methode

```java
public class Main {
    public static void main(String[] args) {
        // Objekt erstellen
        Auto meinAuto = new Auto("Rot");

        // Attribute über Getter auslesen
        System.out.println("Farbe: " + meinAuto.getFarbe());

        // Geschwindigkeit setzen und fahren
        meinAuto.setGeschwindigkeit(50);
        meinAuto.fahre();

        // Auto stoppen
        meinAuto.stoppe();

        // Farbe ändern
        meinAuto.setFarbe("Blau");
        System.out.println("Neue Farbe: " + meinAuto.getFarbe());
    }
}
```

---

### 🔍 Was zeigt dieses Beispiel?

- **Klasse `Auto`** ist der Bauplan.
- **Objekt `meinAuto`** ist eine Instanz dieser Klasse.
- **Attribute** wie `farbe` und `geschwindigkeit` speichern den Zustand.
- **Methoden** wie `fahre()` und `stoppe()` definieren das Verhalten.
- **Konstruktor** initialisiert das Objekt.
- **Getter/Setter** ermöglichen kontrollierten Zugriff auf die Attribute.

---