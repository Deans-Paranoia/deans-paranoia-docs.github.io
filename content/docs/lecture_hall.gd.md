+++
title = "lecture_hall.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node2D](../Node2D)

## Opis
Skrypt odpowiadający za odbycie spotaknia porządkowego, podczas którego Dziekan może dokonać wykreślkenia gracza z listy studentów.
## Opis Właściwości

### npcScene

```gdscript
var npcScene
```

Ładuje scenę postaci NPC

### deanScene

```gdscript
var deanScene
```

Ładuje scenę postaci Deana

### rng

```gdscript
var rng
```

Tworzy nowy generator liczb losowych

### available\_spots

```gdscript
var available_spots
```

Lista dostępnych miejsc

### clicked

```gdscript
var clicked = 0
```

Licznik kliknięć

### kicked\_player\_number

```gdscript
var kicked_player_number = 1
```

Numer gracza do wyrzucenia

### maximum\_ammount\_to\_kick

```gdscript
var maximum_ammount_to_kick = 1
```

Maksymalna liczba do wyrzucenia

### hovered\_student

```gdscript
var hovered_student
```

Zmienna przechowująca informację o najechanym studencie

### students\_to\_kick

```gdscript
var students_to_kick
```

Lista studentów do wyrzucenia

### playersCount

```gdscript
var playersCount = 0
```

Licznik graczy

### endgame

```gdscript
var endgame
```

Ładuje scenę zakończenia gry

### kicked\_notification

```gdscript
var kicked_notification
```

Ładuje scenę powiadomienia o wyrzuceniu

## Opis Metod

### on\_npc\_spawn

```gdscript
func on_npc_spawn()
```

Funkcja wykonująca się przy spawnowaniu npc

### set\_student

```gdscript
func set_student(name, spot)
```

### set\_dean

```gdscript
func set_dean()
```

### on\_student\_moved

```gdscript
func on_student_moved()
```

Funkcja wykonuje się kiedy dziekan przeniesie studenta, żeby go wyrzucić

### on\_student\_catched

```gdscript
func on_student_catched(name)
```

Funkcja wywołuje się przy złapaniu studenta

### quit\_game

```gdscript
func quit_game()
```

### change\_players\_count

```gdscript
func change_players_count()
```

### show\_end\_screen

```gdscript
func show_end_screen()
```

### send\_restart\_task\_call

```gdscript
func send_restart_task_call()
```

### remove\_student\_from\_hall

```gdscript
func remove_student_from_hall(i)
```

### back\_to\_game

```gdscript
func back_to_game(to_kick)
```

### restart\_map

```gdscript
func restart_map()
```

### move\_student

```gdscript
func move_student(name)
```

### set\_hovered\_student

```gdscript
func set_hovered_student(name)
```

ustawanie wybranego studenta

### check\_if\_was\_player

```gdscript
func check_if_was_player(name)
```

Sprawdzanie czy student był graczem czy też botem