# bash_menu_ex

Alternative to bash select.

Highly customizable bash menu. It helps to manage different environment settings.

The idea behind it came to me a few years back when I started to use Linux as my primary development platform. When I was working with multiple projects simultaneously, it often required to set or change a bunch of environment variables, switching from one build toolchain to another, changing the path, adjusting other system settings, etc. It was a real pain in the neck to keep track of all of that, and I did not like the built-in bash select feature mostly from an estetic point of view.

This bash menu was quite an improvement. And in the end, I caught two rabbits, I made my life more comfortable, and I practiced some bash. I was improving on it for quite some time, and I am pretty satisfied with it now.

Here is how all 3 demo modules look in the Linux console:

![image](https://github.com/ademyankov/bash_menu_ex/blob/master/demo_menu.png)

## Demo modules:
- *demo_platform* shows how to use sub (child) menu
- *demo_build* shows how to use check box items
- *demo_logs* shows how to use radio box items and alignment

## Usage
In order to run the demo simply source the menu module and a demo module into
the environment:
```sh
. menu_ex && . demo_platform
dev
```
Or source all 3 demo modules together:
```sh
. menu_ex && . demo_platform && . demo_build && . demo_logs
dev
```
## Aliases
Bash aliases used to show a menu, to select an item, or to execute a callback. The API documentation has all the decription on how to use the menu as well as the demo modules has detailed describtion on how to use the API.
```sh
dev   # Show all the menus
PL    # Show PLATFORM menu
Build # Show Build menu
logs  # Show logs menu
```
To see what aliases available for a specific menu, run a menu's alias with *-h* switch, for example:
```sh
PL -h
```
