# Standard Nori Plugin Layout

## Overview

This is a basic layout for Nori plugin. 

## Go Directories

### `/internal`

Private plugin code. 
This is the code you don't want others importing in their plugins, applications or libraries.
Usually this directory contains implementation of plugin interfaces.

### `/pkg`

Plugin code that's ok to use by other plugins (e.g., `/pkg/myplugin`).
This directory is a good place to describe a public interface provided by the plugin.
Other projects will import these interfaces, structures and data types, so think twice before you put something here.

It's ok not to use it if your plugin implements an external interface.

### `/plugin`

Main plugin code for this project.

