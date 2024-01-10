+++
title = "ReferenceCollector"
description = "To use this tool:  - Place this script and Collector.gd in your Godot project folder. - Open the script in the script editor. - Modify the properties below to control the tool's behavior. - Go to File -> Run to run the script in the editor.\n\nTo use this tool:  - Place this script and Collector.gd in your Godot project folder. - Open the script in the script editor. - Modify the properties below to control the tool's behavior. - Go to File -> Run to run the script in the editor."
author = ""
date = "2024-01-10"
+++

<!-- Auto-generated from JSON by GDScript docs maker. Do not edit this document directly. -->

**Extends:** [EditorScript](../EditorScript)

## Opis

To use this tool:  - Place this script and Collector.gd in your Godot project folder. - Open the script in the script editor. - Modify the properties below to control the tool's behavior. - Go to File -> Run to run the script in the editor.

To use this tool:  - Place this script and Collector.gd in your Godot project folder. - Open the script in the script editor. - Modify the properties below to control the tool's behavior. - Go to File -> Run to run the script in the editor.

## Opis Właściwości

### Collector

```gdscript
var Collector: SceneTree
```

### directories

```gdscript
var directories: Array
```

A list of directories to collect files from.

### is\_recursive

```gdscript
var is_recursive: bool = true
```

If true, explore each directory recursively

### patterns

```gdscript
var patterns: Array
```

A list of patterns to filter files.

### save\_path

```gdscript
var save_path: String = "res://reference.json"
```

Output path to save the class reference.