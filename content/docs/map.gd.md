+++
title = "map.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node2D](../Node2D)

## Opis
Skrypt odpowiadający za wygląd oraz fukcjonalność mapy.
## Opis Właściwości

### studentScene

```gdscript
@export var studentScene: PackedScene
```

Deklaracja zmiennych przechowujących trzy sceny: studentScene, deanScene, npcScene

### deanScene

```gdscript
@export var deanScene: PackedScene
```

### npcScene

```gdscript
@export var npcScene: PackedScene
```

### textures

```gdscript
var textures
```

Inicjalizacja pustej listy 'textures'

### timeUi

```gdscript
var timeUi
```

Ładowanie sceny 'time.tscn' z katalogu 'ui' i tworzenie instancji tej sceny

### isVotingProcess

```gdscript
var isVotingProcess = false
```

Inicjalizacja zmiennej 'isVotingProcess' jako logicznej wartości 'False'

### day

```gdscript
var day = 1
```

Inicjalizacja zmiennej 'day' jako liczby całkowitej równą 1

### rand

```gdscript
var rand
```

Inicjalizacja generatora liczb losowych

## Opis Metod

### restart\_tasks

```gdscript
func restart_tasks()
```

### set\_dean\_position

```gdscript
func set_dean_position(deanId, vector)
```

### restart\_npc

```gdscript
func restart_npc(name, task_number)
```

### set\_time\_ui

```gdscript
func set_time_ui(time)
```

### setNpc

```gdscript
func setNpc(name, task_number, has_name)
```

### setPlayer

```gdscript
func setPlayer(i, task_number)
```

### set\_code\_number

```gdscript
func set_code_number(random, day)
```

### change\_code

```gdscript
func change_code()
```

### set\_npc\_for\_host

```gdscript
func set_npc_for_host(name, task_number, has_name)
```

Parametry: name - imię studenta, task_number - numer taska, które robi student has_name - zmienna bool, mówiąca czy npc już posiada imię Ustawia npc dla hosta.

### change\_view

```gdscript
func change_view()
```

### npcs\_notes

```gdscript
func npcs_notes(isVisible)
```

### npcs\_walking

```gdscript
func npcs_walking(isVisible)
```

### npcs\_computer

```gdscript
func npcs_computer(isVisible)
```

## Sygnały

- signal taskType(taskType): Sygnał 'taskType' emitowany z argumentem 'taskType'
