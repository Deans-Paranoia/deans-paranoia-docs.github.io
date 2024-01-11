+++
title = "lecture_hall.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za odbycie spotaknia porządkowego, podczas którego dziekan może dokonać wykreślenia gracza z listy studentów.
## Opis Właściwości

### npcScene

```gdscript
var npcScene
```

Ładuje scenę postaci NPC.

### deanScene

```gdscript
var deanScene
```

Ładuje scenę postaci Deana.

### rng

```gdscript
var rng
```

Tworzy nowy generator liczb losowych.

### available\_spots

```gdscript
var available_spots
```

Lista dostępnych miejsc.

### clicked

```gdscript
var clicked = 0
```

Licznik kliknięć.

### kicked\_player\_number

```gdscript
var kicked_player_number = 1
```

Numer gracza do wyrzucenia.

### maximum\_ammount\_to\_kick

```gdscript
var maximum_ammount_to_kick = 1
```

Maksymalna liczba graczy do wyrzucenia.

### hovered\_student

```gdscript
var hovered_student
```

Zmienna przechowująca informację o studencie, nad którym gracz będący dziekanem wskazuje kursorem w danej chwili.

### students\_to\_kick

```gdscript
var students_to_kick
```

Lista studentów do wyrzucenia.

### playersCount

```gdscript
var playersCount = 0
```

Licznik graczy.

### endgame

```gdscript
var endgame
```

Ładuje scenę zakończenia gry.

### kicked\_notification

```gdscript
var kicked_notification
```

Ładuje scenę powiadamiającą o wyrzuceniu.

## Opis Metod

### on\_npc\_spawn

```gdscript
func on_npc_spawn()
```

Funkcja wykonująca się przy dodawaniu npc do mapy.

### set\_student

```gdscript
func set_student(name, spot)
```
Ustawia rolę podanego gracza na studenta i jego miejsce na auli.
### set\_dean

```gdscript
func set_dean()
```
Ustawia rolę podanego gracza na dziekana.
### on\_student\_moved

```gdscript
func on_student_moved()
```
Funkcja wykonuje się kiedy dziekan wybierze studenta, aby go wykreślić z listy.

### on\_student\_catched

```gdscript
func on_student_catched(name)
```

Funkcja wywołuje się gdy dziekan próbuje złapać studenta.

### quit\_game

```gdscript
func quit_game()
```
Funkcja zamykająca grę i uruchamijąca scene pokazującą zwycięzcęrozgrywki.
### change\_players\_count

```gdscript
func change_players_count()
```
Zmienia licznik pozostałych studentów (nie botów) pozostałych w grze.
### show\_end\_screen

```gdscript
func show_end_screen()
```
Przełącza widok gracza na scene informującąo zakończeniu i zwycięzcy rozgrywki.
### send\_restart\_task\_call

```gdscript
func send_restart_task_call()
```
Przygotowuje mapę do kolendej rundy.
### remove\_student\_from\_hall

```gdscript
func remove_student_from_hall(i)
```
Usuwa studenta z auli.
### back\_to\_game

```gdscript
func back_to_game(to_kick)
```
Uruchamia funkcje usuwającą graczy z rozgrywki, którzy są na liście do usunięcia. Ponadto Usuwa wszystkie npc, aby można było je na nowo przypisać.
### restart\_map

```gdscript
func restart_map()
```
Przypisuje studentów odpowiednich piętr. Ustawia kamerę gracza, czas rundy, oddaje graczom możliwość poruszania się.
### move\_student

```gdscript
func move_student(name)
```
Wizualnie przesuwa postać wybranego przez dziekana studenta.
### set\_hovered\_student

```gdscript
func set_hovered_student(name)
```
Ustawanie imię wybranego przez dziekana studenta do odpoweidniej zmiennej.

### check\_if\_was\_player

```gdscript
func check_if_was_player(name)
```

Sprawdzanie czy wybrany przez dziekana student był graczem czy botem.