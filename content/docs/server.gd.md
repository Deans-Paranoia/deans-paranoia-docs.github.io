+++
title = "server.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za logike związaną z terminalami oraz kodem do serwera z odpowiedziemi do testów dziekana, ten skrypt ma możliwość zakończenia gry zwycięstwem dla studentów.
## Opis Właściwości

### endgame

```gdscript
var endgame
```
Zmienna przechowująca końcową scenę.
### rng

```gdscript
var rng
```
Generator liczb losowych.
### green\_terminal

```gdscript
var green_terminal
```
Zielony terminal - scena.
### violet\_terminal

```gdscript
var violet_terminal
```
Fioletowy terminal - scena.
### yellow\_terminal

```gdscript
var yellow_terminal
```
Żółty terminal scena.
### terminal1

```gdscript
var terminal1
```
Pierwszy wybrany terminal.
### terminal2

```gdscript
var terminal2
```
Drugi wybrany terminal.
### terminal3

```gdscript
var terminal3
```
Trzeci wybrany terminal.
### serverValue

```gdscript
var serverValue
```
Przechowuje poprawny kod do serwera dziekana.
### digits\_sprites

```gdscript
var digits_sprites
```
Przechowuje obrazki 10 cyfr do wyświetlenia na terminalach.
## Opis Metod

### set\_server\_value

```gdscript
func set_server_value(value)
```
Funkcja ustawiająca wartość poprawnego kodu do serwera dziekana.
### calculate\_value

```gdscript
func calculate_value()
```

Funkcja sprawdzająca poprawność wprowadzonych wartości do 3 terminali.

### run\_server\_error

```gdscript
func run_server_error()
```
Wyświetla animacje na serwerze, informującą od niepoprawnym kodzie.
### set\_terminals\_position\_for\_host

```gdscript
func set_terminals_position_for_host()
```

Funkcja ustawiająca pozycję terminali dla hosta.

### set\_terminals\_position

```gdscript
func set_terminals_position(position1, position2, position3)
```
Funkcja ustawiająca pozycję terminali dla graczy.
### show\_end\_screen

```gdscript
func show_end_screen()
```
Wyświetla ekran końcowy, informujący o zwycięzcy
### on\_number\_changed

```gdscript
func on_number_changed(name, value)
```
Parametry: name - nazwa terminala, value - cyfra Funkcja zmieniająca teksturę cyfr na ekranie w zależności od wartości wprowadzonej do terminali.