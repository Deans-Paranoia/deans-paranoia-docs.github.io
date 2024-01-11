+++
title = "main.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Główny skrypt odpowiedzialny za funkcjonalności sieciowe.
## Opis Właściwości

### Address

```gdscript
@export var Address = ""
```
Address IP serwera
### Port

```gdscript
@export var Port = 8909
```
Port przez który komunukują się host z innymi instancjami gry.
### single\_ip\_info

```gdscript
var single_ip_info
```
Zmienna, która przechowuje informacje o pojedyńczym urządzeniu sieciowym, na którym można utworzyć grę.
### peer

```gdscript
var peer
```
Zmienna przechowująca dane o łączącej się z hostem instancji gry.
## Opis Metod

### peer\_connected

```gdscript
func peer_connected(id: int)
```

Parametry: id - unikalny numer generowany losowo podczas nawiązywania połączenia z seweren. 
Funkcja informująca o nowym graczu, który dołączył jako peer, wywołuje się gdy jest emitowany sygnał wbudowany 'peer_connected'.

### peer\_disconnected

```gdscript
func peer_disconnected(id: int)
```

Parametry: id - unikalny numer generowany losowo podczas nawiązywania połączenia z serwerem.
Funkcja informująca o graczu, który rozłączył się jako peer, wywołuje się gdy jest emitowany sygnał wbudowany 'peer_disconnected'.

### connected\_to\_server

```gdscript
func connected_to_server()
```

Funkcja informująca o graczu, który połączył się do serwera klikając przycisk dołączenia do gry, wywołuje się gdy jest emitowany sygnał wbudowany 'connected_to_server'.

### connection\_failed

```gdscript
func connection_failed()
```

Funkcja informująca o graczu, któremu nie udało się dołączyć do gry. Wywołuje się gdy jest emitowany sygnał wbudowany 'connection_failed'.

### SendPlayerInformation

```gdscript
func SendPlayerInformation(name, id)
```

Parametry: name - nazwa gracza który dołączył do gry, id - unikalny numer generowany losowo podczas nawiązywania połączenia z seweren.
Funkcja wysyłająca informacje o graczu, który połączył się do serwera. Funkcja zapisuje informacje o graczu w skrypcie globalnym

### StartGame

```gdscript
func StartGame()
```
Funkcja wywoływana w momencie rozpoczęcia gry, wyświetla mapę na ekranach graczy.

### hostGame

```gdscript
func hostGame() -> bool
```
Return: bool funkcja wywołująca wbudowane metody multiplayer API, funkcja ta sprawia, że inni użytkownicy mogą zobaczyć serwer.

### update\_dean\_id

```gdscript
func update_dean_id(id)
```
Funkcja zapisuje informacje o nowo wybranym dziekanie do skryptu globalnego.

### on\_update\_id

```gdscript
func on_update_id(id)
```
Funkcja wywoływana w momencie wybrania innej osoby, która ma otrzymać rolę dziekana.

### joinByIp

```gdscript
func joinByIp(ip)
```
Funkcja sprawdzająca czy można dołączyć do serwera, jeśli to możliwe, to takoż czyni.

### on\_start\_game

```gdscript
func on_start_game()
```
Funkcja wywoływana po kliknięciu przycisku rozpoczęcia gry.
Rozpoczyna grę.
### signName

```gdscript
func signName(name_number, i)
```
Funkcja przypisująca graczowi imię spośród wszystkich dostępnych imion studentów.

## Sygnały

- signal current_player(id): 
- signal isServer(): 
- signal gameStart(): 
