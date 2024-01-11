+++
title = "ServerBrowser.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający za wyświetlanie serwera na liście dostępnych z którym obecnie można sie połaczyć oraz informacje o nim.
## Opis Właściwości

### listenPort

```gdscript
@export var listenPort: int = 8911
```
Port nasłuchiwania.
### broadcastPort

```gdscript
@export var broadcastPort: int = 8912
```
Port nadawania
### broadcastAddress

```gdscript
@export var broadcastAddress: String = ""
```
Addres na IP którym jest tworzony serwer.
### serverInfo

```gdscript
@export var serverInfo: PackedScene
```
Informacje o nazwie serwera, jego adresie, liczbie graczy i daje możliwość dołączenia do tego serwera.
### broadcastTimer

```gdscript
var broadcastTimer: Timer
```
Częstotliwość odświeżania informacji z serverInfo.
### RoomInfo

```gdscript
var RoomInfo
```
Spakowane informacje, które klienci orzymują od hosta i na ich podstawie tworzą serverInfo
### playerCount

```gdscript
var playerCount = 0
```
Ilość graczy na serwerze.
### broadcaster

```gdscript
var broadcaster: PacketPeerUDP
```
Zmienna odpowiedzialna za komunikacje po protokole sieciowym UDP.
### listener

```gdscript
var listener: PacketPeerUDP
```
Odpiera inforamcje po UDP.
### is\_host

```gdscript
var is_host = false
```
Flaga informująca czy dana instanacja gry jest hostem.
## Opis Metod

### setBroadcastAddress

```gdscript
func setBroadcastAddress(address: String)
```

Parametry: address - ciąg znaków z adresem IP hostującego Funkcja ustawiająca adres strumieniowanie informacji związanych z aktualnym serwerem gry.

### setUp

```gdscript
func setUp()
```

Funkcja ustawiająca port dla użytkownika, który planuje dołączyć do gry.

### setupBroadcast

```gdscript
func setupBroadcast(name)
```

Funkcja ustawiająca strumieniowanie informacji z serwera do graczy.

### exit\_tree

```gdscript
func exit_tree()
```
Funkcja wywoływana w momencie zamknięcia serwera.

### cleanUp

```gdscript
func cleanUp()
```
Funkcja czyszcząca informacje związane z serwerem.

### joinByIp

```gdscript
func joinByIp(ip)
```
Funkcja wysyłająca sygnał w momencie dołączenia do gry.

## Sygnały

- signal joinGame(ip): 
