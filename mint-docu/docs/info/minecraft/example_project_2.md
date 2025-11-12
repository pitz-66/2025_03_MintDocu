
# Projektstruktur für Ressourcen

    src/main/resources/
    ├── fabric.mod.json
    ├── assets/
    │   └── modid/
    │       ├── blockstates/
    │       │   └── my_block.json
    │       ├── models/
    │       │   ├── block/
    │       │   │   └── my_block.json
    │       │   └── item/
    │       │       └── my_block.json
    │       └── textures/
    │           └── block/
    │               └── my_block.png
    └── data/
        └── modid/
            └── recipes/
                └── my_block.json


## 1. Blockstate-Datei

`assets/modid/blockstates/my_block.json`

```json
{
  "variants": {
    "": { "model": "modid:block/my_block" }
  }
}
```

**Erklärung:**

*   Verweist auf das Blockmodell `modid:block/my_block`.

***

## 2. Blockmodell

`assets/modid/models/block/my_block.json`

```json
{
  "parent": "block/cube_all",
  "textures": {
    "all": "modid:block/my_block"
  }
}
```

**Erklärung:**

*   `cube_all` bedeutet, dass alle Seiten dieselbe Textur verwenden.
*   Texturpfad: `modid:block/my_block`.

***

## 3. Itemmodell

`assets/modid/models/item/my_block.json`

```json
{
  "parent": "modid:block/my_block"
}
```

**Erklärung:**

*   Das Item nutzt das gleiche Modell wie der Block.

***

## 4. Textur

`assets/modid/textures/block/my_block.png`

*   **Format:** PNG, 16×16 Pixel (Standard für Minecraft).
*   **Tipp:** Du kannst eine einfache Farbe oder ein Muster nehmen.
*   Tools: Paint.NET, GIMP oder Online-Editor wie <https://minecraft.novaskin.me/>.

***

## 5. Crafting-Rezept (optional)

`data/modid/recipes/my_block.json`

```json
{
  "type": "minecraft:crafting_shaped",
  "pattern": [
    "##",
    "##"
  ],
  "key": {
    "#": { "item": "minecraft:stone" }
  },
  "result": {
    "item": "modid:my_block",
    "count": 1
  }
}
```

**Erklärung:**

*   2×2 Stein ergibt deinen Block.

***

## Checkliste

*   `fabric.mod.json` enthält deinen Mod-Eintrag.
*   Alle Dateien liegen im richtigen Pfad.
*   Textur ist vorhanden und korrekt benannt.
*   Nach Änderungen: `gradlew runClient` starten.

***

Hier ist die fertige ZIP-Datei mit der vollständigen Ressourcenstruktur, allen JSON-Dateien und einer Beispieltextur (16×16 Pixel, graue Farbe):

[fabric_mod_resources.zip](fabric_mod_resources.zip)

## Inhalt der ZIP:

*   **fabric.mod.json** – Mod-Metadaten
*   **assets/modid/**
    *   `blockstates/my_block.json`
    *   `models/block/my_block.json`
    *   `models/item/my_block.json`
    *   `textures/block/my_block.png` (graue Platzhaltertextur)
*   **data/modid/recipes/my\_block.json** – Crafting-Rezept


