+++
title = "movementInput.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za możliwość i kierunek poruszania sie gracza.
## Opis Właściwości

### player\_name

```gdscript
var player_name: String
```

Nazwa gracza.

### can\_move

```gdscript
var can_move: bool = true
```

Flaga określająca możliwość ruchu postaci.

### last\_direction

```gdscript
var last_direction = "(0, 0)"
```

Zmienna określająca ostatni kierunek ruchu gracza przed zatrzymaniem.

### temp\_speed

```gdscript
var temp_speed
```

Tymczasowa prędkość, używana do zatrzymywania i przywracania ruchu.

### speed

```gdscript
var speed: int = 250
```

Prędkość ruchu gracza.

### canMove

```gdscript
var canMove = true
```

Flaga określająca, czy gracz może się poruszać.

## Opis Metod

### apply\_physics

```gdscript
func apply_physics()
```

Funkcja aplikująca fizykę ruchu gracza.

### calculate\_velocity

```gdscript
func calculate_velocity()
```

Funkcja obliczająca wektor prędkości gracza na podstawie kierunku wynikającego z wciśnietych przez niego klawiszy..

### take\_current\_speed\_value

```gdscript
func take_current_speed_value() -> int
```

Funkcja zwracająca aktualną wartość prędkości gracza.

### stop\_player\_movement

```gdscript
func stop_player_movement()
```

Funkcja zatrzymująca ruch gracza.

### restore\_player\_movement

```gdscript
func restore_player_movement(tempspeed)
```
Przywraca graczowi jego prędkość poruszania się.

### emit\_direction\_signal

```gdscript
func emit_direction_signal(velocity)
```

Funkcja emitująca sygnał informujący o kierunku ruchu gracza.

### stop\_walking\_animation

```gdscript
func stop_walking_animation()
```

Funkcja obsługująca zatrzymanie animacji chodzenia gracza.

## Sygnały

- signal direction(direction_vector): Sygnał informujący o kierunku ruchu postaci.
