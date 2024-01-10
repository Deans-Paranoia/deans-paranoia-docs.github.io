+++
title = "ServerBrowser.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Control](../Control)

## Opis

## Opis Właściwości

### listenPort

```gdscript
@export var listenPort: int = 8911
```

### broadcastPort

```gdscript
@export var broadcastPort: int = 8912
```

### broadcastAddress

```gdscript
@export var broadcastAddress: String = ""
```

### serverInfo

```gdscript
@export var serverInfo: PackedScene
```

### broadcastTimer

```gdscript
var broadcastTimer: Timer
```

### RoomInfo

```gdscript
var RoomInfo
```

### playerCount

```gdscript
var playerCount = 0
```

### broadcaster

```gdscript
var broadcaster: PacketPeerUDP
```

### listener

```gdscript
var listener: PacketPeerUDP
```

### is\_host

```gdscript
var is_host = false
```

## Opis Metod

### setBroadcastAddress

```gdscript
func setBroadcastAddress(address: String)
```

Parametry: address - ciąg znaków z adresem IP hostującego Return: bool Funckja ustawiająca adres strumieniowanie informacji związanych z aktualnym serwerem gry

### setUp

```gdscript
func setUp()
```

funkcja ustawiająca port dla użytkownika, który planuje dołączyć do gry

### setupBroadcast

```gdscript
func setupBroadcast(name)
```

funkcja ustawiająca strumieniowanie informacji z serwera do graczy

### exit\_tree

```gdscript
func exit_tree()
```

funkcja wywoływana w momencie zamknięcia serwera

### cleanUp

```gdscript
func cleanUp()
```

funkcja czyszcząca informacje związane z serwerem

### joinByIp

```gdscript
func joinByIp(ip)
```

funckja wysyłająca sygnał w momencie dołąćzenia do gry

## Sygnały

- signal joinGame(ip): 
