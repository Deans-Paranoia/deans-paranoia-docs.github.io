+++
title = "map.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za wygląd oraz fukcjonalność mapy.
## Opis Właściwości

### studentScene

```gdscript
@export var studentScene: PackedScene
```

Deklaracja zmiennych przechowujących trzy sceny: studentScene, deanScene, npcScene.

### deanScene

```gdscript
@export var deanScene: PackedScene
```
Scena zawierająca wszelkie obiekty związane z dziekanem, tworzące go.
### npcScene

```gdscript
@export var npcScene: PackedScene
```
Scena zawierająca wszelkie obiekty związane z npc, tworzące go.
### textures

```gdscript
var textures
```

Inicjalizacja pustej listy 'textures'.

### timeUi

```gdscript
var timeUi
```
Ładowanie sceny 'time.tscn' z katalogu 'ui' i tworzenie instancji tej sceny. Odpowiada ona za mechanikę czasu rundy.

### isVotingProcess

```gdscript
var isVotingProcess = false
```
Inicjalizacja zmiennej 'isVotingProcess' jako logicznej wartości 'False'. Informuje ona, czy dziekan jest w trakcie wybierania studenta do wykreślenia podczas spotakania porządkowego na auli.

### day

```gdscript
var day = 1
```
Inicjalizacja zmiennej 'day' liczbą całkowitą równą 1. Wskazuje ona na numer rundy gry.

### rand

```gdscript
var rand
```
Inicjalizacja generatora liczb losowych.

## Opis Metod

### restart\_tasks

```gdscript
func restart_tasks()
```
Resetuje zadania przypisane npc.
### set\_dean\_position

```gdscript
func set_dean_position(deanId, vector)
```
zmienia pozycje dziekana na mapie.
### restart\_npc
Usuwa każdego npc z grup danego zadania. Losuje każdemu nowe.
```gdscript
func restart_npc(name, task_number)
```

### set\_time\_ui

```gdscript
func set_time_ui(time)
```
Ustawia czas rundy.
### setNpc

```gdscript
func setNpc(name, task_number, has_name)
```
Ustawia obiekt jako npc.
### setPlayer

```gdscript
func setPlayer(i, task_number)
```
Ustawia obiekt jako gracz.
### set\_code\_number

```gdscript
func set_code_number(random, day)
```
Losuje tablicę do wyświetlenia jednej z 3 cyfr kodu do serwera w zależności od numeru rundy.
### change\_code

```gdscript
func change_code()
```
Zmienia kod na tablicy.
### set\_npc\_for\_host

```gdscript
func set_npc_for_host(name, task_number, has_name)
```
Analogicznie do set\_npc, ale tym razem dla oczu hosta.
Parametry: name - imię studenta, task_number - numer taska, które robi student has_name - zmienna bool, mówiąca czy npc już posiada imię Ustawia npc dla hosta.

### change\_view

```gdscript
func change_view()
```
Zmienia widok dla graczy na aulę.

## Sygnały

- signal taskType(taskType): Sygnał 'taskType' 
Emitowany z argumentem 'taskType'. Niesie informacje o typie zadania.
