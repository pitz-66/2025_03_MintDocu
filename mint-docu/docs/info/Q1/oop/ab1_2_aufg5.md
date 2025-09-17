# Arbeitsblatt 1: Eine Klasse für Bücher

Erstellen Sie eine Klasse Buch, die die Attribute titel, autor und seitenzahl besitzt.
Der Konstruktor bekommt die entsprechenden Attribute als Parameter übergeben. Verwenden Sie private
für die Attribute und implementieren Sie Getter- und Setter-Methoden für die Attribute.
Schreiben Sie eine Main-Methode, in der das Buch „Per Anhalter durch die Galaxis“ von Douglas Adams
mit 240 Seiten erstellt wird. Dabei soll anschließend mit der set-Methode die Seitenzahl auf 256 gesetzt
und der Autor mit Hilfe der get-Methode ausgegeben werden.

```java
public class Buch {
    private String titel;
    private String autor;
    private int seitenzahl;

    public Buch(String titel, String autor, int seitenzahl) {
        this.titel = titel;
        this.autor = autor;
        this.seitenzahl = seitenzahl;
    }

    public String getTitel() {
        return titel;
    }

    public void setTitel(String titel) {
        this.titel = titel;
    }

    public String getAutor() {
        return autor;
    }

    public void setAutor(String autor) {
        this.autor = autor;
    }

    public int getSeitenzahl() {
        return seitenzahl;
    }

    public void setSeitenzahl(int seitenzahl) {
        this.seitenzahl = seitenzahl;
    }

    public static void main(String[] args) {
        Buch buch = new Buch("Per Anhalter durch die Galaxis", "Douglas Adams", 240);
        buch.setSeitenzahl(256);
        System.out.println("Autor: " + buch.getAutor());
    }
}

```