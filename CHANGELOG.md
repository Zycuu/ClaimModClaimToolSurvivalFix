# Changelog

## 1.0.1

Fixed the recipe ingredient format for newer Minecraft data pack parsing.

Changed ingredients from old object entries to string entries:

```json
"ingredients": [
  "minecraft:paper",
  "minecraft:golden_shovel"
]
```

This fixes reload errors where the server reports the shapeless ingredient list as empty.

## 1.0.0

Initial release.

Added a shapeless Paper + Golden Shovel recipe that outputs a gold named Claim Shovel with custom model data 1999 for ClaimMod.
