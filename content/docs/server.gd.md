+++
title = "server.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node2D](../Node2D)

## Opis
Skrypt odpowiadający za logike związana z terrminalami oraz kodem do servera dziekana, ten skrypt ma możliwość zakończenia gry ze zwycieństwem dla studentów.
## Opis Właściwości

### endgame

```gdscript
var endgame
```

### rng

```gdscript
var rng
```

### green\_terminal

```gdscript
var green_terminal
```

### violet\_terminal

```gdscript
var violet_terminal
```

### yellow\_terminal

```gdscript
var yellow_terminal
```

### terminal1

```gdscript
var terminal1
```

### terminal2

```gdscript
var terminal2
```

### terminal3

```gdscript
var terminal3
```

### serverValue

```gdscript
var serverValue
```

### digits\_sprites

```gdscript
var digits_sprites
```

## Opis Metod

### set\_server\_value

```gdscript
func set_server_value(value)
```

### calculate\_value

```gdscript
func calculate_value()
```

Funkcja sprawdzająca poprawność wprowadzonych wartości terminali

### run\_server\_error

```gdscript
func run_server_error()
```

### set\_terminals\_position\_for\_host

```gdscript
func set_terminals_position_for_host()
```

Funkcja ustawiająca pozycję terminali dla hosta

### set\_terminals\_position

```gdscript
func set_terminals_position(position1, position2, position3)
```

### show\_end\_screen

```gdscript
func show_end_screen()
```

### on\_number\_changed

```gdscript
func on_number_changed(name, value)
```

Parametry: name - nazwa terminala, value - cyfra Funkcja zmieniająca teksturę cyfr na ekranie w zależności od wartości wprowadzonej do terminali