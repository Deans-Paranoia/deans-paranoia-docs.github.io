+++
title = "waiting_room.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za wyświetlanie i edycje informacji o rolach jakie otrzymuje każdy z graczy.
## Opis Właściwości

### serverInfo

```gdscript
@export var serverInfo: PackedScene
```

### current

```gdscript
var current: int
```

### dean

```gdscript
var dean: int
```

### isServer

```gdscript
var isServer = false
```

## Opis Metod

### enable\_dean\_change

```gdscript
func enable_dean_change()
```

funkcja która przekazuje pozwolenie na zmianę gracza, który otrzyma rolę dziekana

### makeAsDean

```gdscript
func makeAsDean(id)
```

funkcja przysłająca informacje o wybranym dziekanie

### findDeanId

```gdscript
func findDeanId() -> int
```

Return: int funkcja która szuka osoby, która ma ustawioną rolę dziekan

### refresh\_table

```gdscript
func refresh_table()
```

funckcja odświeża tabelę z graczami - ich nazwą i ich rolą w grze

### on\_current\_player

```gdscript
func on_current_player(id)
```

funkcja wysyłająca informajce o graczu, który obecnie jest wpisywany do tabeli

## Sygnały

- signal button_pressed(node): 
- signal dean_picked(deanId): 
