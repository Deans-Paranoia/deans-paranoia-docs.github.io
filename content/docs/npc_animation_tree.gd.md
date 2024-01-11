+++
title = "npc_animation_tree.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za animacje npc.
## Opis Właściwości

### taskVector

```gdscript
var taskVector = "(0, 0)"
```

Wektor wskazujący bieżące zadanie NPC.

### sprite\_to\_back\_to

```gdscript
var sprite_to_back_to: Sprite2D
```

Sprite, który zostanie przywrócony po zakończeniu wykonywania zadania.

## Opis Metod

### taking\_notes\_loop

```gdscript
func taking_notes_loop()
```

Funkcja obsługująca animacje zadania "takingNotes".

### computer\_loop

```gdscript
func computer_loop()
```

Funkcja obsługująca animacje zadania "computer".

### vending\_machine\_loop

```gdscript
func vending_machine_loop()
```

Funkcja obsługująca animacje zadania "vendingMachine".

### rotate\_npc

```gdscript
func rotate_npc(direction)
```

Funkcja obsługująca obrót NPC.

### set\_vector\_and\_sprite

```gdscript
func set_vector_and_sprite(sprite, vector)
```

Funkcja ustawiająca wektor i sprite postaci NPC.

### run\_animation

```gdscript
func run_animation(taskVector)
```

Funkcja uruchamiająca odpowiednią animację postaci NPC.