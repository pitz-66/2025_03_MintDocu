
# Fabric-Setup in IntelliJ

siehe auch [getting-started](https://docs.fabricmc.net/develop/getting-started/)

## Voraussetzungen

*   **Minecraft Java Edition**
*   **Java 17** (für aktuelle Minecraft-Versionen)
*   **IntelliJ IDEA** (Community oder Ultimate)
*   **Gradle** (wird meist automatisch von IntelliJ gehandhabt)

## Schritt-für-Schritt Setup

1.  **Fabric MDK herunterladen**
    *   Gehe zu <https://fabricmc.net/use/installer/> und lade den **Fabric Mod Development Kit (MDK)** herunter.
    *   Alternativ: <https://github.com/FabricMC/fabric-example-mod>.

2.  **Projekt entpacken und öffnen**
    *   Entpacke das heruntergeladene MDK in einen Ordner.
    *   Öffne IntelliJ und wähle **Open** → den Ordner des Projekts.

3.  **Gradle Sync**
    *   IntelliJ erkennt das Gradle-Projekt automatisch.
    *   Falls nicht: Rechtsklick auf `build.gradle` → **Import Gradle Project**.

4.  **Minecraft Development Plugin (optional)**
    *   Installiere das Plugin **Minecraft Development** in IntelliJ (unter Settings → Plugins).
    *   Erleichtert das Erstellen von Mods und Templates.

5.  **Run Configurations**
    *   Nach dem Sync findest du im Gradle-Toolfenster Tasks wie `runClient`.
    *   Damit kannst du Minecraft direkt aus IntelliJ starten.





