+++
title = "task.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->



## Opis
Skrypt odpowiadający, za uruchamianie animacji wykonywania zadania przez daną postać.
## Opis Metod

### on\_npc\_task\_type\_emitted

```gdscript
func on_npc_task_type_emitted(task_type)
```

Parametry: task_type - typ tasku Funkcja do odtwarzania konkretnego zadania przez gracza.

### run\_task

```gdscript
func run_task(task_type)
```

Parametry: task_type - typ tasku Funkcja dobiera odpowiednią funkcje zależnie od zmiennej task_type.

### task\_computer

```gdscript
func task_computer()
```

Funkcja emitująca sygnał o task_type = computer.

### task\_taking\_notes

```gdscript
func task_taking_notes()
```

Funkcja emitująca sygnał o task_type = takingNotes.

### task\_walking

```gdscript
func task_walking()
```

Funkcja emitująca sygnał o task_type = walking.

### vending\_machine

```gdscript
func vending_machine()
```

Funkcja emitująca sygnał o task_type = vendingMachine.

## Sygnały

- signal npc_walking_task(): 
- signal npc_sprite_task(task_type): 
