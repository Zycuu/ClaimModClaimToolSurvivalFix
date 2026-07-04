# Claim Shovel Recipe

A tiny Minecraft Java data pack that adds a survival crafting recipe for ClaimMod.

## Recipe

Shapeless recipe, works in both the 2x2 player inventory grid and the 3x3 crafting table.

```text
Paper + Golden Shovel = Claim Shovel
```

The crafted item is a `minecraft:golden_shovel` named **Claim Shovel** in gold text.

The output also includes:

```json
"minecraft:custom_model_data": {
  "floats": [1999.0]
}
```

That matches ClaimMod's default `claim_tool_item.custom_model_data: 1999` setting.

## File layout

```text
pack.mcmeta
data/
  claim_shovel_recipe/
    recipe/
      claim_shovel.json
```

## Install

Drop the data pack zip into your server world's `datapacks` folder, then run:

```mcfunction
/reload
/datapack list
```

Players can craft it manually with Paper + Golden Shovel. A single shapeless recipe covers both the 2x2 inventory grid and the 3x3 crafting table.

## Compatibility notes

This pack targets ClaimMod's default config:

```yaml
claim_tool: minecraft:golden_shovel
claim_tool_item:
  custom_model_data: 1999
```

If the server owner changes ClaimMod's `claim_tool` or `claim_tool_item.custom_model_data`, update the recipe output to match.

## Why this exists

ClaimMod already supports a special shovel item, but normal players need a survival way to obtain it. This pack makes the default Claim Shovel craftable with Paper and a Golden Shovel.
