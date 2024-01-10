+++
title = "npc_animation_tree.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [AnimationTree](../AnimationTree)

## Opis

## Opis Właściwości

### taskVector

```gdscript
var taskVector = "(0, 0)"
```

Wektor związany z bieżącym zadaniem postaci NPC.

### sprite\_to\_back\_to

```gdscript
var sprite_to_back_to: Sprite2D
```

Sprite, do którego zostanie przywrócony animowany sprite po zakończeniu zadania.

## Opis Metod

### taking\_notes\_loop

```gdscript
func taking_notes_loop()
```

Metoda obsługująca animacje zadania "takingNotes".

### computer\_loop

```gdscript
func computer_loop()
```

Metoda obsługująca animacje zadania "computer".

### vending\_machine\_loop

```gdscript
func vending_machine_loop()
```

Metoda obsługująca animacje zadania "vendingMachine".

### rotate\_npc

```gdscript
func rotate_npc(direction)
```

Parametry: direction Metoda zdalna obsługująca obrót postaci NPC.

### set\_vector\_and\_sprite

```gdscript
func set_vector_and_sprite(sprite, vector)
```

Parametry: sprite, vector Metoda zdalna ustawiająca wektor i sprite postaci NPC.

### run\_animation

```gdscript
func run_animation(taskVector)
```

Parametry: taskVector Metoda zdalna uruchamiająca odpowiednią animację postaci NPC.