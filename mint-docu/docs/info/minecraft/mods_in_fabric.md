# Mods in frabricmc installieren

In **FabricMC** ist die Installation von Mods sehr einfach, aber sie unterscheidet sich von Forge. Hier sind die Schritte:

***

## 1. Fabric Loader installieren

*   Lade den **Fabric Installer** von <https://fabricmc.net/use/installer/>.
*   Starte den Installer und wähle:
    *   **Minecraft-Version** (z. B. 1.20.1)
    *   **Install Client**
*   Nach der Installation erscheint ein Fabric-Profil im Minecraft-Launcher.

## 2. Fabric API hinzufügen

*   Die meisten Mods benötigen die **Fabric API**.
*   Lade sie von <https://modrinth.com/mod/fabric-api> oder <https://www.curseforge.com/minecraft/mc-mods/fabric-api>.
*   Lege die `.jar`-Datei in den **mods**-Ordner:
        %appdata%/.minecraft/mods   (Windows)
        ~/.minecraft/mods           (Linux/Mac)

## 3. Mods installieren

*   Lade die gewünschten Mods (z. B. von Modrinth oder CurseForge).
*   Stelle sicher, dass:
    *   Die Mod-Version zur **Minecraft-Version** passt.
    *   Die Mod für **Fabric** ist (nicht Forge!).
*   Kopiere die `.jar`-Dateien in den **mods**-Ordner.

## 4. Spiel starten

*   Starte Minecraft mit dem **Fabric-Profil**.
*   Mods werden automatisch geladen.

## 5. Für die Entwicklungsumgebung

*   Wenn du über `gradlew runClient` startest:
    *   Mods müssen in `run/mods` liegen (wird beim ersten Start erstellt).
    *   Fabric API auch hier hinzufügen.

## Liste mit den besten Mods

Hier ist eine Auswahl beliebter und empfehlenswerter **Fabric Mods**, die deine Spiel- und Entwicklererfahrung deutlich verbessern können:

### 🚀 Performance & Optimierung (Must-Haves)

*   **Sodium**: Ersetzt OptiFine für bessere Performance, steigert FPS erheblich [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/s2EpNpjX)
*   **Iris Shaders**: Shader-Unterstützung für Sodium, ermöglicht wunderschöne Shader-Effekte [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/s2EpNpjX)
*   **Lithium**: Optimierungen für KI, Physik und Ticks – flüssigeres Spielgefühl [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/s2EpNpjX)
*   **Starlight**: Überarbeitet das Lichtsystem, sorgt für schnelleres Chunk-Rendering [\[modrinth.com\]](https://modrinth.com/collection/s2EpNpjX)

***

### 🧰 Quality-of-Life & Utilities

*   **Just Enough Items (JEI)**: Zeigt Crafting-Rezepte übersichtlich im Inventar [\[beebom.com\]](https://beebom.com/best-minecraft-fabric-mods/), [\[modrinth.com\]](https://modrinth.com/collection/s2EpNpjX)
*   **Jade**: Zeigt Tooltips zu Blocks und Items beim Drüberfahren [\[modrinth.com\]](https://modrinth.com/collection/s2EpNpjX), [\[modrinth.com\]](https://modrinth.com/collection/GTY3iY8u)
*   **Xaero’s Minimap & Xaero’s World Map**: Minimap plus komplette Weltkarte mit Waypoints [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/GTY3iY8u)
*   **AppleSkin**: Zeigt Hunger-/Sättigungswerte direkt im Food HUD [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/GTY3iY8u)
*   **Mod Menu**: Zeigt installierte Mods im Spielmenü – sehr praktisch [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/GTY3iY8u)

***

### 🎨 Visuelle Features & Immersion

*   **Entity Culling**: Blendet unsichtbare Entities/Blöcke aus – Performance-Boost [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/s2EpNpjX)
*   **Continuity**: Sorgt für nahtlose Texturen durch Connected Textures [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/GTY3iY8u)
*   **3D Skin Layers**: Spieler-Skins in voller 3D-Ansicht im Spiel [\[modrinth.com\]](https://modrinth.com/collection/v9EnAzf9/mods), [\[modrinth.com\]](https://modrinth.com/collection/GTY3iY8u)

***

### 🌍 Welt- und Gameplay-Addons

*   **Essential Mod**: Erlaubt das Hosten und Teilen von Welten im LAN mit eingebauten Emotes [\[beebom.com\]](https://beebom.com/best-minecraft-fabric-mods/), [\[beebom.com\]](https://beebom.com/best-minecraft-fabric-mods/)
*   **Terralith**: Komplett neue Weltgenerierung mit etwa 100 Biomen [\[pingperfect.com\]](https://pingperfect.com/blog/home/best-minecraft-fabric-mods-to-enhance-your-experience/)
*   **When Dungeons Arise**: Fügt riesige, detailreiche Dungeons voller Loot hinzu [\[deltiasgaming.com\]](https://deltiasgaming.com/minecraft-mods-you-need-to-check-out-in-2025/)
*   **Biomes O’ Plenty**: Bringt eine Fülle neuer Biome in Overworld, Nether und End [\[deltiasgaming.com\]](https://deltiasgaming.com/minecraft-mods-you-need-to-check-out-in-2025/)

***

### 📦 Weitere nützliche Bibliotheken

*   **Fabric API**: Grundlegende Bibliothek, unerlässlich für fast alle Fabric-Mods [\[curseforge.com\]](https://www.curseforge.com/minecraft/mc-mods/fabric-api), [\[modrinth.com\]](https://modrinth.com/mod/fabric-api/)
*   **Cloth Config API**, **Architectury**, **FerriteCore**: Support-Bibliotheken für andere Mods [\[modrinth.com\]](https://modrinth.com/mods)

***



