# mc-sound-seeds
Last updated: Minecraft 1.19.4

### Information
In Minecraft 1.19 a seed is now provided with sent sounds to be used to randomly pick which variant of a sound is chosen.
This as a result allows the variants to be consistent between clients.

Using the seeds in **sound_seeds.json** will allow you to play the specific variant in a sound.

This may be useful for thing like music sounds, which play custom random tracks.

**Note (pre 1.19.1): https://bugs.mojang.com/browse/MC-253055 will cause sound seeds to appear different for players with resource packs.**

### Format
```json
{
  "minecraft:entity.sheep.shear": {
    "sounds": [
      {
        "id": "minecraft:mob/sheep/shear",
        "seed": 826277665134049000
      }
    ]
  },
  "minecraft:entity.panda.step": {
    "sounds": [
      {
        "id": "minecraft:mob/panda/step1",
        "seed": 5069112585259837000
      },
      {
        "id": "minecraft:mob/panda/step2",
        "seed": 1166111593840821800
      },
      {
        "id": "minecraft:mob/panda/step3",
        "seed": -2657126373912257500
      },
      {
        "id": "minecraft:mob/panda/step4",
        "seed": -5790529243937572000
      },
      {
        "id": "minecraft:mob/panda/step5",
        "seed": 6185334978411823000
      }
    ]
  }
}
```

For example, when sending the sound ``minecraft:entity.panda.step`` to the client use the seed ``5069112585259837000`` to cause the
``minecraft:mob/panda/step1`` variant to play.
