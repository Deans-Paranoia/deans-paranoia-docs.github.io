+++
title = "terminal.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za informacje wyświetlane na terminalach.
## Opis Właściwości

### actual\_value

```gdscript
var actual_value = 0
```
Zmienna przechowująca aktualną wartość wyświetlaną na terminalu.
### textures

```gdscript
var textures
```
Zmienna przechowująca dostępne tekstury dla terminali (liczby i kolory).
### can\_update\_value

```gdscript
var can_update_value: bool = false
```
Flaga określająca, czy gracz może zmienić cyfrę na terminalu.
## Opis Metod

### load\_textures

```gdscript
func load_textures()
```

Funkcja ładująca teksturę.

### update\_texture

```gdscript
func update_texture()
```

Funkcja aktualizująca teksturę terminala.

### use\_terminal

```gdscript
func use_terminal()
```
Gdy gracz chce wejść w interakcje z terminalem, funkcja uruchamia odpowiednie fragmenty kodu, odpowiedzialne za zmianę cyfry na nim.
### show\_terminal

```gdscript
func show_terminal(name)
```
Zmiennia widoczność teminala na mapie.
## Sygnały

- signal change_number(name, value): 
