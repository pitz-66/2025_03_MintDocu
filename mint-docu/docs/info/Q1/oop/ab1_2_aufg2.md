# Arbeitsblatt 1: eine Klasse für den Baum

Implementieren Sie eine Klasse Baum mit den Attributen blattform, rinde und höhe sowie
den Methoden blaetterAustreiben() und blaetterAbwerfen(). Die Methoden bekommen jeweils den
Parameter Jahreszeit übergeben und geben ein true oder false als Ausgabewert zurück.
Außerdem soll der Konstruktor implementiert werden, bei dem die Attribute als Parameter übergeben werden.


```java

class Baum {
    String blattform;
    String rinde;
    Float hoehe;

    public Baum(String blattform, String rinde, Float hoehe) {
        this.blattform = blattform;
        this.rinde = rinde;
        this.hoehe = hoehe;
    }

    public Boolean blaetterAustreiben(String jahreszeit) {
        // der lange weg mit if... else..
        if (jahreszeit == "Fruehling") {
            return true;
        }
        else {
            return false;
        }
    }

    public Boolean blaetterAbwerfen(String jahreszeit) {
        // so geht es viel einfacher
        return jahreszeit == "Herbst";
    }
}


public class Wald {
    public static void main(String[] args) {
        Baum meinBaum = new Baum("rund", "rau", (float)5.5);
        System.out.println(meinBaum.blaetterAustreiben("Fruehling"));
        System.out.println(meinBaum.blaetterAbwerfen("Herbst"));
        System.out.println("Hallo Baum");

    }
}


```