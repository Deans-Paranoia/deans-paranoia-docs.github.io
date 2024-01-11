+++
title = "deanInput.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za czynności wykonywane przez gracza sterującego dziekanem.
## Opis Właściwości

### catch\_info\_instance

```gdscript
var catch_info_instance
```

Instancja widżetu odpowiadającego za informacje o złapaniu studenta.

### is\_tablet\_open

```gdscript
var is_tablet_open: bool = false
```

Flaga określająca, czy tablet dziekana jest otwarty.

### scene

```gdscript
var scene
```

Gotowy widget sceny tabletu.

### tablet\_scene

```gdscript
var tablet_scene
```

Scena tabletu.

### is\_task\_area

```gdscript
var is_task_area
```

Zmienna określająca, czy dziekan znajduje się w obszarze zadania.

### body

```gdscript
var body: CharacterBody2D
```

Referencja do ciała postaci.

### can\_use\_alarm

```gdscript
var can_use_alarm: bool = false
```

Flaga określająca, czy Dean może aktywować alarm przeciwpożarowy.

## Opis Metod

### change\_alarm\_state

```gdscript
func change_alarm_state()
```

Funkcja obsługująca zmianę stanu alarmu przeciwpożarowego.

### manage\_deans\_tablet

```gdscript
func manage_deans_tablet()
```

Funkcja zarządzająca widżetem tabletu dziekana.

## Sygnały

- signal student_picked(): Sygnał informujący o wybraniu studenta.
- signal student_catched(name): Sygnał informujący o złapaniu studenta. Przekazuje nazwę złapanego studenta.
