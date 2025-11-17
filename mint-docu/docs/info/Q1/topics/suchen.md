# Suchalgorithmen

## Lineare Suche (Sequential Search)

**Beschreibung:**

*   Die lineare Suche ist das einfachste Suchverfahren.
*   Sie geht Element für Element durch die Liste und vergleicht jedes mit dem gesuchten Wert.
*   Wenn das Element gefunden wird, gibt die Methode den Index zurück, ansonsten ein Hinweis, dass es nicht existiert.
*   **Komplexität:**
    *   **Best Case:** O(1) (gesuchtes Element ist am Anfang)
    *   **Worst Case:** O(n) (gesuchtes Element ist am Ende oder nicht vorhanden)

**Wann sinnvoll?**

*   Bei **unsortierten Listen** oder kleinen Datenmengen.

**Python-Beispiel:**

```python
def lineare_suche(liste, ziel):
    for index, wert in enumerate(liste):
        if wert == ziel:
            return index
    return -1  # -1 bedeutet: nicht gefunden

# Beispiel
daten = [3, 7, 1, 9, 5]
print(lineare_suche(daten, 9))  # Ausgabe: 3
print(lineare_suche(daten, 4))  # Ausgabe: -1
```

## Binäre Suche (Binary Search)

**Beschreibung:**

*   Die binäre Suche funktioniert nur auf **sortierten Listen**.
*   Sie teilt die Liste wiederholt in zwei Hälften:
    1.  Vergleicht das mittlere Element mit dem Ziel.
    2.  Wenn das Ziel kleiner ist, wird die linke Hälfte durchsucht, sonst die rechte.
*   **Komplexität:**
    *   **Best Case:** O(1)
    *   **Worst Case:** O(log n)

**Wann sinnvoll?**

*   Bei **großen, sortierten Datenmengen**.

**Python-Beispiel:**

```python
def binaere_suche(liste, ziel):
    links, rechts = 0, len(liste) - 1
    while links <= rechts:
        mitte = (links + rechts) // 2
        if liste[mitte] == ziel:
            return mitte
        elif liste[mitte] < ziel:
            links = mitte + 1
        else:
            rechts = mitte - 1
    return -1  # nicht gefunden

# Beispiel
daten = [1, 3, 5, 7, 9, 11]
print(binaere_suche(daten, 7))  # Ausgabe: 3
print(binaere_suche(daten, 4))  # Ausgabe: -1
```

Hier ist eine leicht verständliche Erklärung zur **Suche mit Hashfunktion** sowie ein Python-Beispiel:

***

## Suche mit Hashfunktion (Hash-basierte Suche)

**Beschreibung:**

*   Bei der Hash-basierten Suche wird eine **Hash-Tabelle** verwendet.
*   Eine Hashfunktion berechnet aus dem Schlüssel (z. B. einem Wert) einen Index, unter dem die Daten gespeichert werden.
*   Dadurch kann das gesuchte Element in **konstanter Zeit O(1)** gefunden werden (im Durchschnitt).
*   **Vorteile:** Sehr schnell für große Datenmengen.
*   **Nachteile:**
    *   Benötigt zusätzlichen Speicher.
    *   Bei Kollisionen (zwei Werte haben denselben Hash) muss eine Strategie wie Verkettung oder lineares Sondieren genutzt werden.

**Wann sinnvoll?**

*   Wenn schnelle Zugriffe auf Daten erforderlich sind, z. B. bei großen Mengen von Schlüssel-Wert-Paaren.

***

### **Python-Beispiel:**

Wir nutzen ein Dictionary (eingebaute Hash-Tabelle in Python):

```python
# Erstellen einer Hash-Tabelle (Dictionary)
hash_tabelle = {
    "Apfel": 1,
    "Banane": 2,
    "Kirsche": 3
}

# Suchfunktion unter Verwendung der Hash-Tabelle
def suche_mit_hash(hash_tabelle, schluessel):
    return hash_tabelle.get(schluessel, -1)  # -1 bedeutet: nicht gefunden

# Beispiel
print(suche_mit_hash(hash_tabelle, "Banane"))  # Ausgabe: 2
print(suche_mit_hash(hash_tabelle, "Orange"))  # Ausgabe: -1
```

***

### **Eigene Hashfunktion + einfache Implementierung:**

```python
# Einfache Hashfunktion: Summe der ASCII-Werte modulo Größe der Tabelle
def einfache_hashfunktion(schluessel, groesse):
    return sum(ord(c) for c in schluessel) % groesse

# Implementierung einer Hash-Tabelle mit Verkettung
class HashTabelle:
    def __init__(self, groesse):
        self.groesse = groesse
        self.tabelle = [[] for _ in range(groesse)]

    def einfuegen(self, schluessel, wert):
        index = einfache_hashfunktion(schluessel, self.groesse)
        # Prüfen, ob Schlüssel schon existiert
        for i, (k, v) in enumerate(self.tabelle[index]):
            if k == schluessel:
                self.tabelle[index][i] = (schluessel, wert)
                return
        self.tabelle[index].append((schluessel, wert))

    def suchen(self, schluessel):
        index = einfache_hashfunktion(schluessel, self.groesse)
        for k, v in self.tabelle[index]:
            if k == schluessel:
                return v
        return -1  # nicht gefunden

# Beispiel
ht = HashTabelle(10)
ht.einfuegen("Apfel", 1)
ht.einfuegen("Banane", 2)
ht.einfuegen("Kirsche", 3)

print(ht.suchen("Banane"))  # Ausgabe: 2
print(ht.suchen("Orange"))  # Ausgabe: -1
```
