+++
title = "chat.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [CanvasLayer](../CanvasLayer)

## Opis

## Opis Właściwości

### new\_message

```gdscript
@export var new_message: PackedScene
```

Zmienna przechowująca scenę dla nowej wiadomości

### line\_edit

```gdscript
var line_edit
```

Referencja do kontrolki wprowadzania tekstu

### message\_panel

```gdscript
var message_panel
```

Referencja do panelu wiadomości

### chat\_in\_use

```gdscript
var chat_in_use: bool = false
```

Flaga określająca, czy czat jest aktualnie używany

## Opis Metod

### add\_message\_to\_chat

```gdscript
func add_message_to_chat(message_content, name)
```

Funkcja dodająca wiadomość do czatu (zdalnie wywoływana)

## Sygnały

- signal chat_opened(is_opened): Sygnał informujący o otwarciu lub zamknięciu czatu
