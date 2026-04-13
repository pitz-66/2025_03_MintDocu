---
tags:
  - Datenbanken
  - ER-Diagramme
  - SQL
  - Aufgaben
---

# Aufgaben – Relationale Datenbanken & ER-Diagramme

Zwölf Aufgaben zu den Themen Datenbankmodellierung, ER-Diagramme und relationale Schemas.  
Klappe die jeweilige Lösung auf, um die Beispielantwort zu sehen.

---

## Aufgabe 1 – Begriffe zuordnen

!!! question "Aufgabe"
    Erkläre in eigenen Worten die folgenden Begriffe und nenne jeweils ein konkretes Beispiel aus einer Schulverwaltung:

    - Entität
    - Attribut
    - Primärschlüssel
    - Fremdschlüssel
    - Relation (Tabelle)

??? success "Lösung"
    | Begriff | Erklärung | Beispiel |
    |---|---|---|
    | **Entität** | Ein eindeutig identifizierbares Objekt der realen Welt | „Simon Müller" ist eine Entität des Typs *Schüler* |
    | **Attribut** | Eine Eigenschaft einer Entität | Vorname, Nachname, Geburtsdatum eines Schülers |
    | **Primärschlüssel** | Attribut, das jeden Datensatz eindeutig identifiziert | `ID_Schüler` – keine zwei Schüler haben dieselbe ID |
    | **Fremdschlüssel** | Verweist auf den Primärschlüssel einer anderen Tabelle | `ID_Klasse` in der Schüler-Tabelle → Klassen-Tabelle |
    | **Relation / Tabelle** | Darstellung eines Entitätstyps als Tabelle mit Spalten (Attribute) und Zeilen (Datensätze) | Die Tabelle `Schüler` |

---

## Aufgabe 2 – Primär- und Fremdschlüssel identifizieren

!!! question "Aufgabe"
    Gegeben sind folgende drei Tabellen einer Bibliotheksdatenbank. Benenne jeweils den Primärschlüssel und alle Fremdschlüssel:

    - **Buch**: ISBN, Titel, Erscheinungsjahr, ID_Autor  
    - **Autor**: ID_Autor, Nachname, Vorname, Geburtsjahr  
    - **Ausleihe**: ID_Ausleihe, ISBN, ID_Leser, Ausleihdatum, Rückgabedatum

??? success "Lösung"
    **Tabelle: Buch**

    | Spalte | Rolle |
    |---|---|
    | **ISBN** | :key: Primärschlüssel |
    | Titel, Erscheinungsjahr | Normale Attribute |
    | *ID_Autor* | :link: Fremdschlüssel → Autor |

    **Tabelle: Autor**

    | Spalte | Rolle |
    |---|---|
    | **ID_Autor** | :key: Primärschlüssel |
    | Nachname, Vorname, Geburtsjahr | Normale Attribute |

    **Tabelle: Ausleihe**

    | Spalte | Rolle |
    |---|---|
    | **ID_Ausleihe** | :key: Primärschlüssel |
    | *ISBN* | :link: Fremdschlüssel → Buch |
    | *ID_Leser* | :link: Fremdschlüssel → Leser |
    | Ausleihdatum, Rückgabedatum | Normale Attribute |

---

## Aufgabe 3 – Beziehungstypen bestimmen

!!! question "Aufgabe"
    Bestimme den Beziehungstyp (1:1, 1:n oder n:m) für die folgenden Sachverhalte und begründe deine Antwort:

    1. Ein Schüler gehört zu einer Klasse. Eine Klasse hat viele Schüler.
    2. Ein Lehrer kann viele Fächer unterrichten. Ein Fach kann von vielen Lehrern unterrichtet werden.
    3. Jeder Mitarbeiter hat genau einen Mitarbeiterausweis und umgekehrt.
    4. Ein Arzt behandelt viele Patienten. Ein Patient kann von mehreren Ärzten behandelt werden.
    5. Ein Bestellkopf gehört zu genau einem Kunden. Ein Kunde kann viele Bestellungen aufgeben.

??? success "Lösung"
    | Sachverhalt | Typ | Begründung |
    |---|---|---|
    | Schüler ↔ Klasse | **1 : n** | 1 Klasse hat n Schüler, jeder Schüler gehört zu genau 1 Klasse |
    | Lehrer ↔ Fach | **n : m** | Viele Lehrer können dasselbe Fach unterrichten, ein Lehrer kann viele Fächer haben |
    | Mitarbeiter ↔ Ausweis | **1 : 1** | Genau eine Zuordnung in beide Richtungen |
    | Arzt ↔ Patient | **n : m** | Ein Arzt behandelt viele Patienten, ein Patient kann mehrere Ärzte haben |
    | Kunde ↔ Bestellung | **1 : n** | 1 Kunde hat n Bestellungen, jede Bestellung gehört zu genau 1 Kunden |

---

## Aufgabe 4 – ER-Diagramm lesen und beschreiben

!!! question "Aufgabe"
    Gegeben ist ein ER-Diagramm mit den Entitäten **Student** (Attribute: Matrikel-Nr, Name) und **Kurs** (Attribute: Kurs-ID, Bezeichnung). Die Beziehung „belegt" verbindet beide mit der Kardinalität **n:m**. An der Beziehung selbst hängt das Attribut **Note**.

    Beantworte folgende Fragen:

    - Welche Entitäten sind dargestellt?
    - Um welchen Beziehungstyp handelt es sich?
    - Was bedeutet das Attribut „Note" an der Beziehung?
    - Wie viele Tabellen entstehen beim Überführen in ein relationales Schema?

??? success "Lösung"
    - **Entitäten:** `Student` (Matrikel-Nr, Name) und `Kurs` (Kurs-ID, Bezeichnung)

    - **Beziehungstyp:** n:m – ein Student belegt viele Kurse, ein Kurs wird von vielen Studenten belegt

    - **Attribut „Note" an der Beziehung:** Die Note gehört nicht zum Studenten oder Kurs allein, sondern zur konkreten Belegung. Ein Student hat in einem bestimmten Kurs eine bestimmte Note. Solche **Beziehungsattribute** werden in der Zwischentabelle gespeichert.

    - **Anzahl Tabellen:** 3 Tabellen entstehen:

    | Tabelle | Spalten |
    |---|---|
    | Student | **Matrikel-Nr**, Name |
    | Kurs | **Kurs-ID**, Bezeichnung |
    | belegt | ***Matrikel-Nr***, ***Kurs-ID***, Note |

    !!! tip "Hinweis"
        Bei einer n:m-Beziehung entsteht immer eine Zwischentabelle. Attribute der Beziehung selbst gehören in diese Zwischentabelle.

---

## Aufgabe 5 – ER-Diagramm in Tabellen überführen

!!! question "Aufgabe"
    Überführe die folgende Beschreibung in ein relationales Datenbankschema:

    > Ein **Verein** hat viele **Mitglieder**. Jedes Mitglied gehört zu genau einem Verein.
    > Jedes Mitglied kann an mehreren **Veranstaltungen** teilnehmen, und jede Veranstaltung wird von mehreren Mitgliedern besucht.
    > Bei der Teilnahme wird die **Teilnahmegebühr** gespeichert.
    >
    > - Verein: ID, Name, Gründungsjahr  
    > - Mitglied: Mitglieds-ID, Vor- und Nachname  
    > - Veranstaltung: Veranstaltungs-ID, Titel, Datum

??? success "Lösung"
    Es entstehen **4 Tabellen**: Verein, Mitglied, Veranstaltung und die Zwischentabelle Teilnahme.

    **Verein**

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | **ID_Verein** | INT | PK |
    | Name | VARCHAR | |
    | Gründungsjahr | INT | |

    **Mitglied**

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | **ID_Mitglied** | INT | PK |
    | Vorname | VARCHAR | |
    | Nachname | VARCHAR | |
    | *ID_Verein* | INT | FK → Verein (1:n) |

    **Veranstaltung**

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | **ID_Veranstaltung** | INT | PK |
    | Titel | VARCHAR | |
    | Datum | DATE | |

    **Teilnahme** *(Zwischentabelle für n:m)*

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | ***ID_Mitglied*** | INT | PK + FK → Mitglied |
    | ***ID_Veranstaltung*** | INT | PK + FK → Veranstaltung |
    | Teilnahmegebühr | DECIMAL | Beziehungsattribut |

---

## Aufgabe 6 – Normalformen bestimmen

!!! question "Aufgabe"
    Prüfe die folgende Tabelle auf Verstöße gegen die 1., 2. und 3. Normalform und beschreibe, wie du sie in eine normalisierte Form bringst:

    | Bestell-ID | Kunde | Kunden-PLZ | Kunden-Ort | Artikel | Artikelpreis |
    |---|---|---|---|---|---|
    | 1 | Müller | 59872 | Meschede | Stuhl, Tisch | 200, 500 |
    | 2 | Schmidt | 59823 | Arnsberg | Lampe | 80 |
    | 3 | Müller | 59872 | Meschede | Schrank | 1200 |

??? success "Lösung"
    **Verstöße:**

    | Normalform | Verstoß |
    |---|---|
    | **1NF verletzt** | Spalten „Artikel" und „Artikelpreis" enthalten mehrere Werte pro Zelle (Bestell-ID 1) |
    | **2NF verletzt** | Artikelpreis hängt nur vom Artikel ab, nicht von der Bestell-ID → Teilabhängigkeit |
    | **3NF verletzt** | Kunden-Ort hängt von Kunden-PLZ ab, nicht direkt von Bestell-ID → transitive Abhängigkeit |

    **Normalisierte Tabellen (3NF):**

    === "Kunde"
        | **ID_Kunde** | Name | *PLZ* |
        |---|---|---|
        | 1 | Müller | 59872 |
        | 2 | Schmidt | 59823 |

    === "PLZ_Ort"
        | **PLZ** | Ort |
        |---|---|
        | 59872 | Meschede |
        | 59823 | Arnsberg |

    === "Artikel"
        | **ID_Artikel** | Bezeichnung | Preis |
        |---|---|---|
        | 1 | Stuhl | 200 |
        | 2 | Tisch | 500 |
        | 3 | Lampe | 80 |
        | 4 | Schrank | 1200 |

    === "Bestellung"
        | **ID_Bestellung** | *ID_Kunde* |
        |---|---|
        | 1 | 1 |
        | 2 | 2 |
        | 3 | 1 |

    === "Bestellposition"
        | ***ID_Bestellung*** | ***ID_Artikel*** |
        |---|---|
        | 1 | 1 |
        | 1 | 2 |
        | 2 | 3 |
        | 3 | 4 |

---

## Aufgabe 7 – Is-a-Beziehung modellieren

!!! question "Aufgabe"
    In einem Krankenhaus gibt es **Personen**, die entweder **Ärzte** oder **Patienten** sind.

    - Alle Personen haben: Personalnummer, Vorname, Nachname, Geburtsdatum
    - Ärzte haben zusätzlich: Fachgebiet, Dienstbeginn
    - Patienten haben zusätzlich: Krankenkasse, Aufnahmedatum

    Überführe das Modell in relationale Tabellen.

??? success "Lösung"
    Die Is-a-Beziehung (Generalisierung) führt zu **3 Tabellen**. Der Primärschlüssel der Untertypen ist gleichzeitig Fremdschlüssel auf den Obertyp.

    **Person** *(Obertyp)*

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | **Personalnummer** | INT | PK |
    | Vorname | VARCHAR | |
    | Nachname | VARCHAR | |
    | Geburtsdatum | DATE | |

    **Arzt** *(Untertyp)*

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | ***Personalnummer*** | INT | PK + FK → Person |
    | Fachgebiet | VARCHAR | |
    | Dienstbeginn | DATE | |

    **Patient** *(Untertyp)*

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | ***Personalnummer*** | INT | PK + FK → Person |
    | Krankenkasse | VARCHAR | |
    | Aufnahmedatum | DATE | |

    !!! tip "Hinweis"
        Gemeinsame Daten (Name, Geburtsdatum) werden durch diese Struktur **nur einmal** in der Tabelle `Person` gespeichert und nicht redundant wiederholt.

---

## Aufgabe 8 – Schwachen Entitätstyp erkennen

!!! question "Aufgabe"
    In einem Hotel gibt es mehrere **Etagen**. Jede Etage hat mehrere **Zimmer**. Ein Zimmer wird durch seine **Zimmernummer** identifiziert, die aber nur innerhalb einer Etage eindeutig ist (in jeder Etage gibt es ein Zimmer 1, 2, 3, …).

    - Warum ist `Zimmer` ein schwacher Entitätstyp?
    - Wie wird der Primärschlüssel der Tabelle `Zimmer` gebildet?
    - Zeige die resultierenden Tabellen.

??? success "Lösung"
    **Warum schwacher Entitätstyp?**  
    Die Zimmernummer allein ist **nicht eindeutig** – „Zimmer 1" gibt es in jeder Etage. Ohne die Etage kann ein Zimmer nicht identifiziert werden. Ein schwacher Entitätstyp existiert nur in Abhängigkeit eines starken Entitätstyps.

    **Primärschlüssel:**  
    Zusammengesetzt aus `ID_Etage` + `Zimmernummer` – erst die Kombination ist eindeutig.

    **Etage** *(starker Entitätstyp)*

    | Spalte | Schlüssel |
    |---|---|
    | **ID_Etage** | PK |
    | Bezeichnung | |

    **Zimmer** *(schwacher Entitätstyp)*

    | Spalte | Schlüssel |
    |---|---|
    | ***ID_Etage*** | PK + FK → Etage |
    | **Zimmernummer** | PK (partiell) |
    | Kapazität | |

    !!! info "ER-Diagramm"
        Im ER-Diagramm wird der schwache Entitätstyp durch ein **doppeltes Rechteck** und die identifizierende Beziehung durch eine **doppelte Raute** dargestellt.

---

## Aufgabe 9 – Mehrwertiges Attribut modellieren

!!! question "Aufgabe"
    Eine Person kann mehrere **E-Mail-Adressen** haben. 

    - Erkläre, warum das ein Problem für die 1. Normalform darstellt.
    - Zeige, wie das mehrwertige Attribut korrekt in Tabellen überführt wird.

??? success "Lösung"
    **Problem – Verstoß gegen die 1NF:**  
    Die 1. Normalform fordert, dass jede Spalte nur **atomare** (unteilbare) Werte enthält. Mehrere E-Mail-Adressen in einer Spalte zu speichern verletzt diese Regel.

    **Falsch** :x:

    | ID_Person | Name | E-Mail |
    |---|---|---|
    | 1 | Müller | max@web.de, max@gmail.de |

    **Richtig – eigene Tabelle** :white_check_mark:

    **Person**

    | **ID_Person** | Name |
    |---|---|
    | 1 | Müller |

    **Person_Email**

    | ***ID_Person*** | E-Mail-Adresse |
    |---|---|
    | 1 | max@web.de |
    | 1 | max@gmail.de |

    !!! info "ER-Diagramm"
        Im ER-Diagramm wird ein mehrwertiges Attribut durch eine **doppelte Ellipse** dargestellt.

---

## Aufgabe 10 – Rekursive Beziehung modellieren

!!! question "Aufgabe"
    In einer Firma ist jeder **Mitarbeiter** einem Vorgesetzten zugeordnet – der selbst auch ein Mitarbeiter ist. Der oberste Chef hat keinen Vorgesetzten.

    - Wie nennt man diese Art von Beziehung?
    - Wie wird sie in einer Tabelle dargestellt?
    - Welcher Wert steht beim obersten Chef in der Vorgesetzten-Spalte?

??? success "Lösung"
    - **Bezeichnung:** Rekursive Beziehung (auch: Selbstbeziehung) – eine Entität steht mit sich selbst in Beziehung.

    - **Darstellung:** Ein Fremdschlüssel in derselben Tabelle, der auf den Primärschlüssel **derselben** Tabelle verweist.

    - **Oberster Chef:** `NULL` – es gibt keinen Vorgesetzten.

    **Mitarbeiter**

    | **ID_Mitarbeiter** | Name | Abteilung | *ID_Vorgesetzter* |
    |---|---|---|---|
    | 1 | Becker | Leitung | `NULL` |
    | 2 | Müller | Vertrieb | 1 |
    | 3 | Schmidt | Vertrieb | 2 |

    !!! tip "Hinweis"
        `ID_Vorgesetzter` ist ein Fremdschlüssel, der auf `ID_Mitarbeiter` in *derselben* Tabelle verweist. Das nennt man eine **Selbstreferenz**.

---

## Aufgabe 11 – Fehler in einem Datenbankschema finden

!!! question "Aufgabe"
    Das folgende Datenbankschema enthält **vier Fehler**. Finde sie und erkläre jeweils, warum es ein Fehler ist:

    ```
    Schüler  (ID_Schüler, Vorname, Nachname, ID_Klasse)
    Klasse   (ID_Klasse, Bezeichnung, Vorname_Lehrer, Nachname_Lehrer, Fach1, Fach2, Fach3)
    Note     (Note, ID_Schüler, ID_Prüfung)
    ```

??? success "Lösung"
    | # | Fehler | Erklärung |
    |---|---|---|
    | 1 | **Redundanz** | `Vorname_Lehrer` und `Nachname_Lehrer` stehen direkt in der Klassen-Tabelle. Lehrerdaten sollten in eine eigene Tabelle `Lehrer` ausgelagert werden (Verstoß gegen 3NF). |
    | 2 | **Mehrwertige Spalten** | `Fach1`, `Fach2`, `Fach3` sind mehrwertige Attribute als separate Spalten. Das verletzt die **1NF**. Lösung: eigene Tabelle `Fach` mit Verknüpfungstabelle. |
    | 3 | **Fehlender Primärschlüssel** | In der Tabelle `Note` fehlt ein eindeutiger Primärschlüssel. Die Kombination `(ID_Schüler, ID_Prüfung)` sollte als zusammengesetzter PK definiert werden. |
    | 4 | **Irreführender Spaltenname** | Die Spalte heißt `Note` – genauso wie die Tabelle. Das führt zu Verwechslungen. Besser: `Notenwert`. |

---

## Aufgabe 12 – Vollständiges ER-Diagramm entwerfen

!!! question "Aufgabe"
    Entwirf ein vollständiges ER-Diagramm (Chen-Notation) und das zugehörige relationale Schema für folgende Situation:

    > In einem **Sportverein** gibt es **Mitglieder** und **Sportarten**.  
    > Jedes Mitglied kann mehrere Sportarten betreiben, und jede Sportart wird von mehreren Mitgliedern ausgeübt.  
    > Dabei wird gespeichert, seit wann ein Mitglied eine Sportart betreibt (**Eintrittsdatum**).  
    > Jede Sportart wird von einem **Trainer** geleitet. Ein Trainer kann mehrere Sportarten leiten.  
    > Ein Trainer ist selbst kein Mitglied.
    >
    > **Attribute:**  
    > Mitglied (ID, Name, Geburtsdatum) · Sportart (ID, Bezeichnung, Halle) · Trainer (ID, Name, Lizenz)

??? success "Lösung"
    **Beziehungen im Überblick:**

    | Entität A | Beziehung | Entität B | Typ | Besonderheit |
    |---|---|---|---|---|
    | Mitglied | betreibt | Sportart | n:m | Attribut: Eintrittsdatum |
    | Trainer | leitet | Sportart | 1:n | FK in Sportart |

    **Relationale Tabellen:**

    **Mitglied**

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | **ID_Mitglied** | INT | PK |
    | Name | VARCHAR | |
    | Geburtsdatum | DATE | |

    **Trainer**

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | **ID_Trainer** | INT | PK |
    | Name | VARCHAR | |
    | Lizenz | VARCHAR | |

    **Sportart**

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | **ID_Sportart** | INT | PK |
    | Bezeichnung | VARCHAR | |
    | Halle | VARCHAR | |
    | *ID_Trainer* | INT | FK → Trainer (1:n) |

    **betreibt** *(Zwischentabelle n:m)*

    | Spalte | Typ | Schlüssel |
    |---|---|---|
    | ***ID_Mitglied*** | INT | PK + FK → Mitglied |
    | ***ID_Sportart*** | INT | PK + FK → Sportart |
    | Eintrittsdatum | DATE | Beziehungsattribut |

    !!! tip "Zusammenfassung der Regeln"
        - **1:n** → Fremdschlüssel auf der n-Seite (`ID_Trainer` in `Sportart`)
        - **n:m** → Zwischentabelle mit beiden Fremdschlüsseln als zusammengesetztem PK
        - **Beziehungsattribute** (hier: `Eintrittsdatum`) gehören in die Zwischentabelle