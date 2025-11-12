# Erster Mod – Einfacher Block

## Ziel

Wir erstellen einen Mod, der einen neuen Block hinzufügt.

## Schritt-für-Schritt

1.  **Mod-ID und Basis-Klasse**
    *   In `src/main/java/com/deinname/modid/` eine Klasse `ExampleMod.java` anlegen:

```java
package com.deinname.modid;

import net.fabricmc.api.ModInitializer;
import net.minecraft.block.Block;
import net.minecraft.block.Material;
import net.minecraft.util.Identifier;
import net.minecraft.util.registry.Registry;

public class ExampleMod implements ModInitializer {
    public static final String MOD_ID = "modid";

    // Neuer Block
    public static final Block MY_BLOCK = new Block(Block.Settings.of(Material.STONE).strength(4.0f));

    @Override
    public void onInitialize() {
        Registry.register(Registry.BLOCK, new Identifier(MOD_ID, "my_block"), MY_BLOCK);
    }
}
```

***

2.  **`fabric.mod.json` anpassen**
    *   In `src/main/resources/fabric.mod.json`:

```json
{
  "schemaVersion": 1,
  "id": "modid",
  "version": "1.0.0",
  "name": "Mein erster Fabric Mod",
  "description": "Ein einfacher Block-Mod",
  "authors": ["Dein Name"],
  "entrypoints": {
    "main": [
      "com.deinname.modid.ExampleMod"
    ]
  },
  "depends": {
    "fabricloader": ">=0.14.0",
    "minecraft": ">=1.20.1"
  }
}
```

***

3.  **Block-Item hinzufügen (damit man ihn im Inventar sieht)**

```java
import net.minecraft.item.BlockItem;
import net.minecraft.item.Item;
import net.minecraft.item.ItemGroup;

@Override
public void onInitialize() {
    Registry.register(Registry.BLOCK, new Identifier(MOD_ID, "my_block"), MY_BLOCK);
    Registry.register(Registry.ITEM, new Identifier(MOD_ID, "my_block"),
        new BlockItem(MY_BLOCK, new Item.Settings().group(ItemGroup.BUILDING_BLOCKS)));
}
```

***

4.  **Ressourcen hinzufügen**
    *   `src/main/resources/assets/modid/blockstates/my_block.json`
    *   `src/main/resources/assets/modid/models/block/my_block.json`
    *   `src/main/resources/assets/modid/textures/block/my_block.png` (dein Texturbild)

***

✅ Danach: `gradlew runClient` starten → dein Block ist im Spiel!

