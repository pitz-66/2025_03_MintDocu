# Arbeitsblatt 2: UML Klassendiagramme

In Apotheken ersetzen immer häufiger Computersysteme mit angeschlossenen Roboterarmen die klassischen langen
Schieberegale. Das System übernimmt hierbei automatisiert das Suchen und Ausgeben der Arzneien sowie das Ermitteln
von knappen Arzneien, damit diese rechtzeitig nachbestellt werden können. Im Folgenden soll eine vereinfachte
Arzneiverwaltung für maximal 100 Arzneien modelliert werden. Bei den Arzneien wird der eindeutige Name der Arznei,
die Anzahl der vorrätigen Packungen, ihr Preis und die Verschreibungspflicht erfasst. Der Name wird beim Anlegen 
einer neuen Arznei festgelegt und muss anschließend nicht mehr geändert werden. Die Anzahl der Packungen einer
Arznei soll über eine Methode ändereAnzahlUm(…) um einen bestimmten Wert erhöht bzw. verringert werden können.
Der Preis und die Verschreibungspflicht sollen über geeignete Methoden gesetzt und alle Eigenschaften sollen über
geeignete Methoden abgefragt werden können. Die Arzneiverwaltung verwaltet die Arzneien als Feld, verfügt über
eine Methode ausgeben(…) zum Ausgeben einer einzelnen Packung einer Arznei mit einem bestimmten Namen (Material),
eine Methode auffüllen(…) zum Auffüllen einer bestimmten Arznei mit einer Anzahl neuer Packungen und eine Methode
aufnehmen(…) zum Aufnehmen einer neuen Arznei in das System. Wird eine Arznei mit der Methode löschen(…) aus dem
Sortiment gelöscht, entsteht eine Lücke im Feld, die zu einem späteren Zeitpunkt von einer neuen Arznei gefüllt
werden kann.

1) Modellieren Sie die Klassen Arzneiverwaltung und Arznei mit allen Attributen und Methoden inklusive Parametern als UML-Klassendiagramm.
2) Erläutern Sie die von Ihnen ausgewählte Klassenbeziehung.

```puml

class Arznei {
    - name: String
    - anzahl: int
    - preis: double
    - verschreibungspflichtig: boolean
    + Arznei(name: String, anzahl: int, preis: double, verschreibungspflichtig: boolean)
    + aendereAnzahlUm(menge: int): void
    + getName(): String
    + getAnzahl(): int
    + getPreis(): double
    + getVerschreibungspflichtig(): boolean
    + setAnzahl(anzahl: int): void
    + setPreis(preis: double): void
}

class Arneimittelverwaltung {
    - arzneien: Arznei[100]
    + ausgeben(Arznei: arznei): void
    + auffuellen(Arznei: arznei, menge: int): void
    + aufnehmen(Arznei: arznei): void
    + löschen(Arznei: arznei): void
}

Arneimittelverwaltung --> Arznei

```
![ab2_aufg1.puml](ab2_aufg1.puml)

Zu den möglichen Beziehungen im Detail:
[Klassenbeziehungen](https://blog.visual-paradigm.com/de/what-are-the-six-types-of-relationships-in-uml-class-diagrams/)

...ich würde mal sagen, dass es sich hier um eine Aggregationsbeziehung handelt.