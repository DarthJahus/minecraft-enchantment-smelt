# Smelt Enchantment
Pickaxe enchantment that has a chance to **smelt ores on mine**, dropping the ingot instead of the raw material.  
Compatible with **Fortune**. Incompatible with **Silk Touch**.

**Namespace:** `smelt_enchantment:smelt`

## Effect
When mining supported ores without Silk Touch, each level of Smelt gives a chance to drop the **smelted** product instead of the raw ore. Fortune still applies to both paths.

| Level | Smelt chance |
|-------|--------------|
| 1     | 25 %         |
| 2     | 50 %         |
| 3     | 75 %         |
| 4     | 100 %        |

### Supported ores
| Block | Normal drop | With Smelt (on success) |
|-------|-------------|-------------------------|
| Iron Ore / Deepslate Iron Ore | Raw Iron | Iron Ingot |
| Gold Ore / Deepslate Gold Ore | Raw Gold | Gold Ingot |
| Copper Ore / Deepslate Copper Ore | Raw Copper | Copper Ingot |

Mining also plays a short **flame / smoke** particle effect and a quiet fire ambient sound on the block.

## Compatibility
- **Supported:** Pickaxes (`#minecraft:pickaxes`)
- **Compatible with:** Fortune, Unbreaking, Mending, Efficiency, …
- **Incompatible with:** Silk Touch
- **In Enchanting Table:** No
- **Obtainable via:** Treasure loot, traded equipment, villager trades, random loot

## Give
```mcfunction
/give @s enchanted_book[stored_enchantments={"smelt_enchantment:smelt":4}]
```
