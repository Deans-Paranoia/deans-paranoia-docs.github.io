+++
title = "global.gd"
description = ""
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [Node](../Node)

## Description

## Property Descriptions

### Players

```gdscript
var Players
```

Słownik przechowujący informacje o graczach

### deanId

```gdscript
var deanId: int
```

Identyfikator dziekana

### studentsNames

```gdscript
var studentsNames
```

Lista dostępnych nazw studentów

### usedNames

```gdscript
var usedNames
```

Lista użytych nazw studentów

### Tasks

```gdscript
var Tasks: Array
```

Lista dostępnych zadań

### UsedTasks

```gdscript
var UsedTasks: Array
```

Lista użytych zadań

## Method Descriptions

### remove\_name

```gdscript
func remove_name(nameNumber: int)
```

Funkcja dodająca zwolnioną nazwę studenta do listy dostępnych nazw

### resetTasks

```gdscript
func resetTasks()
```

Funkcja resetująca listę zadań, przenosząca zadania z UsedTasks z powrotem do Tasks

### get\_task\_data

```gdscript
func get_task_data(task_number: int) -> Task
```

Funkcja zwracająca dane o zadaniu o określonym numerze

### manage\_task

```gdscript
func manage_task(task_number: int)
```

Funkcja zarządzająca zadaniem o określonym numerze

### remove\_task

```gdscript
func remove_task(task_number: int)
```

Funkcja usuwająca zadanie o określonym numerze z listy dostępnych zadań

## Sub\-classes

### Task

#### Property Descriptions

### positionX

```gdscript
var positionX: float
```

### positionY

```gdscript
var positionY: float
```

### taskType

```gdscript
var taskType: String
```

#### Method Descriptions

### \_init

```gdscript
func _init(positionX, positionY, taskType) -> Task
```

Inicjalizator klasy Task