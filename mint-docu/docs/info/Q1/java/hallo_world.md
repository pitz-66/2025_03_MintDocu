# Hallo World in Java

## Was man wissen muß:

Will man ein Java-Programm direkt ausführen, muss man in der Datei eine Klasse mit den folgenden
Eigenschaften schreiben:

- Der Name der Klasse ist der gleiche wie der Dateiname
- Die Klasse ist `public` - d.h. sie ist von aussen sichtbar
- In der Klasse wird eine Methode implementiert mit dem Namen `main`
- auch die Methode ist natürlich `public`
- sie ist auch `static`, d.h. es ist eine 'Klassen-Methode' und kann damit direkt aufgerufen werden
- Die Methode bekommt als Parameter ein Array of Strings - die Kommandozeilenparameter - die wir hier aber noch nicht verwenden
- Für die Ausgabe verwenden wir `System.out.println()`
- `System` gehört zum Basis-Sprachumfang und muss nicht importiert werden
- in `println` steht das ln für line und fügt der Ausgabe immer ein 'Newline' hinzu.


```java
public class hello_world {
    public static void main(String[] args) {
        System.out.println("hello world");
        String[] my_strings = {"eins", "zwei", "drei"};
        for(int i = 0; i< my_strings.length; i++) {
            System.out.println(my_strings[i]);
        }
    }
}

```


