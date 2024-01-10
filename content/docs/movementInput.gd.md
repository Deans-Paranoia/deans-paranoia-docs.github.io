+++
title = "movementInput.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [CharacterBody2D](../CharacterBody2D)

## Opis

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

Metoda aplikująca fizykę ruchu gracza.

### calculate\_velocity

```gdscript
func calculate_velocity()
```

Parametry: None Return: Wektor prędkości gracza Metoda obliczająca wektor prędkości gracza na podstawie kierunku z wejścia.

### take\_current\_speed\_value

```gdscript
func take_current_speed_value() -> int
```

Return: Prędkość gracza Metoda zwracająca aktualną wartość prędkości gracza.

### stop\_player\_movement

```gdscript
func stop_player_movement()
```

Metoda zatrzymująca ruch gracza.

### restore\_player\_movement

```gdscript
func restore_player_movement(tempspeed)
```

Parametry: tempspeed Metoda przywracająca ruch gracza.

### emit\_direction\_signal

```gdscript
func emit_direction_signal(velocity)
```

Parametry: velocity - wektor prędkości Funkcja emitująca sygnał informujący o kierunku ruchu.

### stop\_walking\_animation

```gdscript
func stop_walking_animation()
```

Metoda zdalna obsługująca zatrzymanie animacji chodzenia gracza.

## Sygnały

- signal direction(direction_vector): Sygnał informujący o kierunku ruchu postaci.
