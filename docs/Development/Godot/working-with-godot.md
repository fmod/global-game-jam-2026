---
title: Working With Godot
layout: default
parent: Development Team
nav_order: 3.3
---
# Working with Godot

## Note
While we do not have an official integration for Godot Engine the [Utopia-Rise FMOD-GDExtension](https://github.com/utopia-rise/fmod-gdextension) is receiving regular updates. We will do our best to support you however we can! Their integration docs can be found [here](https://fmod-gdextension.readthedocs.io/en/latest/).

More info here: [FMOD Forums](https://qa.fmod.com/t/possibility-of-official-support-for-the-godot-engine/19333/21)

## Source Control
We recommend adding the following to your Github `.gitignore` for the Godot FMOD integration:
```
# Keep FMOD addon (plugin + native libs)
!/addons/fmod/**
!/addons/fmod/**/**

# Keep FMOD banks
!/Banks/**
!/Banks/**/**
```
[Godot Ignore File](godot-ignore.html)