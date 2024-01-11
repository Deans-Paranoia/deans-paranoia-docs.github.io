+++
title = "studentInput.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za sterowanie studentem przez gracza.
## Opis Właściwości

### dig\_info\_instance

```gdscript
var dig_info_instance
```
Gotowa zmienna przechowująca instancję sceny dig_and_dean_catch_info, która będzie używana do wyświetlania informacji o kopaniu i złapaniu przez dziekana.

### current\_task\_area

```gdscript
var current_task_area = ""
```
Zmienna przechowująca aktualną strefę zadania gracza. Pusty string, jeśli gracz nie wykonuje zadania.

### fourthFloor

```gdscript
var fourthFloor
```
Gotowa zmienna przechowująca scenę czwartego piętra.

### thirdFloor

```gdscript
var thirdFloor
```
Gotowa zmienna przechowująca scenę trzeciego piętra.

### dangerScene

```gdscript
var dangerScene = "<PackedScene#-9223367941569842968>"
```
Gotowa zmienna przechowująca scenę informującą o wyjściu przez gracza poza obszar zadania.

### danger\_instance

```gdscript
var danger_instance
```
Zmienna do przypisania instancji sceny dangerScene.

### task\_finished

```gdscript
var task_finished = true
```
Flaga określająca, czy zadanie gracza zostało zakończone.

### catchable

```gdscript
var catchable: bool = false
```
Flaga określająca, czy student może zostać złapany przez dziekana.

### is\_catched

```gdscript
var is_catched: bool = false
```
Flaga określająca, czy student został już złapany.

### can\_use\_alarm

```gdscript
var can_use_alarm: bool = false
```
Flaga określająca, czy gracz znajduje się w strefie, gdzie można aktywować alarm.

### multiplayerId

```gdscript
var multiplayerId
```
Identyfikator wieloosobowy gracza.

### can\_use\_server

```gdscript
var can_use_server: bool = false
```
Flaga określająca, czy gracz znajduje się w strefie, gdzie można użyć serwera.

### can\_use\_server\_again

```gdscript
var can_use_server_again: bool = true
```
Flaga określająca, czy gracz może ponownie użyć serwera.

### level

```gdscript
var level: int = 3
```
Zmienna przechowująca numer piętra na którym gracz się znajduje.

### can\_use\_elevator

```gdscript
var can_use_elevator: bool = false
```
Flaga określająca, czy gracz znajduje się w strefie, gdzie można użyć windy.

### can\_use\_booster

```gdscript
var can_use_booster: bool = false
```
Flaga określająca, czy gracz znajduje się w strefie, gdzie można użyć boostera.

### has\_booster

```gdscript
var has_booster: bool = false
```
Flaga określająca, czy student posiada boostera.

### can\_use\_terminal

```gdscript
var can_use_terminal: bool = false
```

Flaga określająca, czy gracz znajduje się w strefie, gdzie można użyć terminalu.

### terminal\_address

```gdscript
var terminal_address
```
Adres terminala, którego gracz potencjalnie może użyć.

### fire\_alarm\_reference

```gdscript
var fire_alarm_reference
```
Referencja do obiektu obsługującego alarm przeciwpożarowy.

### temp\_speed

```gdscript
var temp_speed
```
Zmienna przechowująca tymczasową prędkość ruchu.

### body

```gdscript
var body: CharacterBody2D
```
Referencja do ciała postaci (CharacterBody2D) - potrzebna do poruszania się oraz kolizji.

## Opis Metod

### change\_alarm\_state

```gdscript
func change_alarm_state()
```

Ta funkcja obsługuje włączanie alarmu przeciwpożarowego.

### removeBooster

```gdscript
func removeBooster()
```

Ta funkcja usuwa boostera z mapy, jeśli istnieje.

### sabotage\_alarm

```gdscript
func sabotage_alarm()
```

Funkcja do sabotowania alarmu przez studenta, zatrzymuje na chwile ruch gracza.

### task\_execution

```gdscript
func task_execution()
```
Funkcja do wykonywania taska przez studenta, wysyła sygnał w jakiej strefie znajduje sie gracz.

### catch\_student

```gdscript
func catch_student()
```
Funkcja wywołuje podfunkcje, które razem z nią tworzą pełną logikę łapania studenta przez dziekana.

### use\_server

```gdscript
func use_server()
```
Funkcja do używania serwera przez studenta, sprawdza czy wpisany kod jest poprawny.

### use\_elevator

```gdscript
func use_elevator(side)
```
Funkcja do korzystania z windy, przenosi gracza na odpowiednie piętro, bierze pod uwagę z której strony gracz wsiada do windy.

### acquire\_booster

```gdscript
func acquire_booster()
```

Funkcja nadająca booster studentowi.

### teleport

```gdscript
func teleport(ammount)
```
Teleportuje gracza o wektor podany w parametrze ammount.

### dig

```gdscript
func dig()
```
Wyszukuje przeszkody w pobliżu i uruchamia kopanie, jeśli gracz jest skierowany w stronę przeszkody i naciśnięto przycisku spacji.

### stop\_dig

```gdscript
func stop_dig()
```
Zatrzymuje proces kopania i wyłącza związany z nim timer.

### change\_catchable

```gdscript
func change_catchable(boolean)
```
Funkcja zmienia flagę: czy student może zostać złapany.

### change\_is\_catched

```gdscript
func change_is_catched()
```
Funkcja zmieniająca stan zmiennej is_catched na true. Określa gracza jako złapanego przez dziekana.

### stop\_player\_movement

```gdscript
func stop_player_movement()
```
Funkcja do zatrzymania ruchu studenta, pobiera aktualną predkość i przechowuje ja w temp_speed.

### remove\_obstacle

```gdscript
func remove_obstacle(_obstacle_to_destroy)
```
Funkcja usuwa obiekt na podstawie przekazanej referencji do tego obiektu.

## Sygnały

```gdscript
signal player_task(task_type)
```
Sygnał emitowany, gdy gracz otrzymuje nowe zadanie. Parametr task_type określa typ zadania.
```gdscript
signal disable_player_movement_for_duration(duration)
```
Sygnał emitowany w celu wyłączenia ruchu gracza na określony czas. 
Parametr duration określa długość wyłączenia.
```gdscript
signal use_chat(name)
```
Sygnał używany do uruchomienia czatu. Parametr name określa nazwę czatu.
```gdscript
signal exit_chat(name)
```
Sygnał używany do wyjścia z czatu. Parametr name określa nazwę czatu.
