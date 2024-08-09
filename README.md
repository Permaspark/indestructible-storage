# Indestructible Storage

A small datapack designed to prevent the destruction of valuable items for the 1.20.1 version of Minecraft. 

Includes Shulker Boxes and Player Heads by default for compatibility with the Pebbles Backpacks mod, but is easily configurable. Changes the invulnerability of dropped entities to be indefinite until picked up again, and adds a glowing particle for easy location.

Any additional entries will be added to the main.mcfunction file, in the following format:
```
execute as @e[type=item,nbt]{Item:{id:"<block_name>"},Invulnerable:0b}] at @s run data merge entity @s {Invulnerable:1,Age:-32768}
```

Feel free to use this pack on any singleplayer worlds or servers!
