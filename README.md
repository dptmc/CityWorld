#### CityWorld...

DaddyChurchill always said: The great outdoors is all good and fine but sometimes you just want to go to town. Not any town will do, how about one that goes on forever or multiple ones separated by the largest mountains possible in Minecraft. But what is under those mountains? There is an entire world to explore, have fun!

#### SlimeDog fork

#### Modifications to support MC 1.18
- Compile with Java 17
- Set api-version: 1.18
- Update materials
  - Material.GRASS_PATH -> Material.DIRT_PATH
- Update biomes
  - Biome.BIRCH_FOREST_HILLS -> Biome.BIRCH_FOREST
  - Biome.DESERT_HILLS -> Biome.DESERT
  - Biome.SNOWY_MOUNTAINS -> Biome.SNOWY_SLOPES
  - Biome.TAIGA_HILLS -> Biome.WINDSWEPT_HILLS

#### Code modifications to please SlimeDog
- Roads
  - GRAY_CONCRETE
  - SMOOTH_QUARTZ
  - STONE_BRICK_SLAB
- Lampposts
  - lightpostHeight = 4
  - lightpostbaseMaterial = Material.STONE_BRICKS
  - lightpostMaterial = Material.IRON_BARS

#### Configuration modifications to please SlimeDog
-BuildingWalls/BuildingFoundation/BuildingCeilings/BuildingRoofs
  - Add 1.18 materials
  - Remove
    - concrete and concrete_powder
    - netherrack
    - non-monochromatic terracotta
    - planks
    - weathered copper variants
