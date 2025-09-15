# Was man über Java wissen muss

## Datentypen

Es gibt in Java zwei unterschiedliche Arten die `primitive Data Types` und die `complex Data Types`.

### Primitive Data Types


- boolean
- byte
- short
- int (integer)
- long
- float
- double
- char

im Gegensatz zu Python gibt es also gleich drei Typen für ganze Zahle (short, int, long) mit unterschiedlichem Wertebereich.
Auch für Gleitkommazahlen gibt es zwei Typen (float, double) mit unterschiedlicher Genauigkeit.

### Complex Data Types

...sind letztendlich Objekte. Die wichtigsten sind

- String
- Array

Dabei ist ein Array eine Liste von Variablen gleichen Typs und über den Basistyp mit angehängten [] definiert:

String[] farben = {"blau", "rot", "gelb", "lila"};

int[] zahlen = {5, 10, 15, 20};

auch Klassen und Objekte sind in Java komplexe Datentypen. Man kann diese Typen auch als Referenzdatentypen bezeichnen,
da hier die Variablen nicht den eigentlichen Wert enthält, sondern nur einen `Zeiger` auf das Objekt oder allgemeiner
die Datenstruktur.

### Wrapper-Klassen

In Java kann man auch die einfachen Datentypen zu Objekten machen: Mit Wrapper-Klassen. Hier ein einfaches Beispiel für

```java

int zahl = 500;
Integer zahlInteger = new Integer(zahl);

```
Die Variable zahlInteger ist nun ein Objekt vom Typ Integer. Wozu ist das gut? Solche Objekte können hilfreiche
Methoden besitzen z.B. zur Typumwandlung. Sie können auch den Wert `Null` annehmen, was einfache Datentypen nicht können
`Null` ist dabei nicht zu verwechseln mit dem Integer Wert 0.




## Variablen

Variablen müssen in java - anders als in Python - 'deklariert' werden. Dabei wird ihnen ein Typ zugewiesen:

```java

String hallo = "Hallo";
int alter = 17;

```

Java ist auch 'Typsicher' d.h. man kann einer Variable vom Typ String nicht einfach ein Integer zuweisen - was in Python ja geht.

Es gibt aber die Möglichkeit der Typumwandlung ähnlich wie in Python.


## Kommentare

werden mit // eingeleitet. Bis zum Zeilenende ist dann alles Kommentar.

