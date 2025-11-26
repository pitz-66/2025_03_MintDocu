# Selbst erstelltes Mod installieren

Um dein Fabric-Mod aus IntelliJ so zu verpacken, dass er vom Fabric-Loader erkannt und installiert werden kann, musst du im Wesentlichen ein korrektes **Mod-JAR** mit der richtigen Struktur und den erforderlichen Metadaten erstellen. Hier sind die Schritte:


### ✅ 1. **Projektstruktur prüfen**

Dein Projekt sollte ungefähr so aussehen:

    src/main/java/...         → Dein Mod-Code
    src/main/resources/
        fabric.mod.json        → Mod-Metadaten
        META-INF/
            mods.toml (optional)

Die wichtigste Datei ist **`fabric.mod.json`**, die den Mod beschreibt. Beispiel:

```json
{
  "schemaVersion": 1,
  "id": "meinmod",
  "version": "1.0.0",
  "name": "Mein Mod",
  "description": "Ein Beispiel-Mod",
  "authors": ["Dein Name"],
  "environment": "*",
  "entrypoints": {
    "main": [
      "com.deinname.meinmod.Main"
    ]
  },
  "depends": {
    "fabricloader": ">=0.14.0",
    "minecraft": ">=1.20.1"
  }
}
```

### ✅ 2. **Gradle verwenden (empfohlen)**

Fabric-Mods werden typischerweise mit **Gradle** gebaut. Falls du IntelliJ nutzt, kannst du das Fabric-Example-Mod als Vorlage nehmen. Wichtige Schritte:

*   In `build.gradle` sicherstellen:

```gradle
plugins {
    id 'fabric-loom' version '1.6-SNAPSHOT'
}

group = 'com.deinname'
version = '1.0.0'

dependencies {
    minecraft "com.mojang:minecraft:1.20.1"
    mappings loom.officialMojangMappings()
    modImplementation "net.fabricmc:fabric-loader:0.14.22"
}
```

*   Dann im Terminal:

```bash
./gradlew build
```

Das erzeugt unter `build/libs/` eine JAR-Datei, die du in den `mods`-Ordner von Minecraft legen kannst.


### ✅ 3. **Wichtige Punkte**

*   **fabric.mod.json** muss im JAR enthalten sein (unter `resources`).
*   Der **Entry Point** (z. B. `Main`-Klasse) muss die Fabric-API nutzen und korrekt registriert sein.
*   Keine IntelliJ-spezifischen Dateien (wie `.idea`) im JAR.
*   Falls du Assets (Textures, Sounds) hast, müssen sie unter `resources/assets/<modid>/` liegen.


