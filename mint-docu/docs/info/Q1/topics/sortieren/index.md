# Sortieralgorithmen

Gute Übersicht: [Einfache Sortierverfahren, Hasso-Plattner-Institut](https://hpi.de/friedrich/teaching/units/einfache-sortierverfahren.html)

- [Bubble sort](sortieren_bubblesort.md)
- [Selection sort](sortieren_selectionsort.md)
- [Insertion sort](sortieren_insertionsort.md)

Vergleich:

| Algorithmus       | Komplexität (Best) | Komplexität (Worst) | Stabilität | Vorteile                                  | Nachteile                                   |
|-------------------|---------------------|-----------------------|------------|-------------------------------------------|---------------------------------------------|
| Bubble Sort       | O(n)              | O(n²)                | Ja         | Einfach zu verstehen                     | Sehr langsam bei großen Listen             |
| Selection Sort    | O(n²)             | O(n²)                | Nein       | Wenige Tauschoperationen                 | Immer ineffizient, auch bei sortierten Daten |
| Insertion Sort    | O(n)              | O(n²)                | Ja         | Gut für kleine oder fast sortierte Listen | Langsam bei großen, unsortierten Listen    |


