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
Zmienna przechowująca scenę zawierającą informacje o serwerze.
### current

```gdscript
var current: int
```
Zmienna przechowująca który z graczy pochodzi z tej instancji gry.
### dean

```gdscript
var dean: int
```
Identyfikator gracza będącego dziekanem.
### isServer

```gdscript
var isServer = false
```
Zmienna przechowująca która z instancji gry jest hostem.
## Opis Metod

### enable\_dean\_change

```gdscript
func enable_dean_change()
```
Funkcja która przekazuje pozwolenie na zmianę gracza, który ma otrzymać rolę dziekana.

### makeAsDean

```gdscript
func makeAsDean(id)
```
Funkcja przysłająca informacje o nowo wybranym dziekanie.

### findDeanId

```gdscript
func findDeanId() -> int
```
Funkcja która szuka gracza, która ma ustawioną rolę dziekana.

### refresh\_table

```gdscript
func refresh_table()
```
Funckcja odświeża tabelę z graczami - ich nazwą oraz rolą w grze.

### on\_current\_player

```gdscript
func on_current_player(id)
```
Funkcja wysyłająca informajce o graczu, który obecnie jest wpisywany do tabeli.

## Sygnały

- signal button_pressed(node): 
- signal dean_picked(deanId): 
