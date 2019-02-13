Authors: Johannes Bunk

E-Mail: bunk@uni-bremen.de

Date: December 2018  

Versions: UE 4.20 

This plugin is an example for a simple UI that can be toggled and used to call functions and change maps in a packaged project. It is important to keep in mind, that it only works in standalone mode. 

# General Information:

## Game Instance

* Since we want to save variables that we still want to access after the map has been changed and also maybe want to have a multiplayer option in the future, a costume game instance called "MenuGI" is needed. 

* Opening new maps and sessions is alot easier and less prone to bugs in blueprints, so the game instance functions are all BlueprintImplementable. 

* The blueprint class created from MenuGI is called "MyMenuGI". Don't forget to set it as the projects used game instance in the project settings. 

* The game instance only works as intended in standalone mode. In the editor it will just crash. 

## Level Blueprint

* Toggling the UI is currently handled by the level blueprint. In this folder you can find a picture of how such a blueprint implementation could look like. 

## Multiplayer

* The menu has some multiplayer code left in it. If it is part of the UI, like buttons, it was commented out. Otherwise the functions are still there but never called. 

* These functions are leftovers of an older project and weren't deleted in case multiplayer is ever required in the future. 
