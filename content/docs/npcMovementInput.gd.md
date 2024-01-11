+++
title = "npcMovementInput.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za ruch botów przy wykonywanych taskach.
## Opis Właściwości

### speed

```gdscript
var speed = 400
```

Prędkość ruchu postaci NPC.

### destination

```gdscript
var destination = "(0, 0)"
```

Wektor docelowy dla ruchu postaci NPC.

### point\_A

```gdscript
var point_A: Vector2
```

Punkt A na trasie ruchu postaci NPC.

### point\_B

```gdscript
var point_B: Vector2
```

Punkt B na trasie ruchu postaci NPC.

### move\_direction

```gdscript
var move_direction = "(1, 0)"
```

Wektor kierunku ruchu postaci NPC.

### can\_move

```gdscript
var can_move: bool
```

Flaga określająca możliwość ruchu postaci NPC.

### walking\_task

```gdscript
var walking_task = false
```

Flaga określająca, czy postać NPC jest w trakcie zadania polegającego na poruszaniu się.

### rng

```gdscript
var rng
```
Generator liczb losowych.

## Opis Metod

### wait

```gdscript
func wait()
```

Funkcja zatrzymująca NPC.

## Sygnały

- signal rotate(direction): Sygnał informujący o zmianie kierunku obrotu postaci NPC.
