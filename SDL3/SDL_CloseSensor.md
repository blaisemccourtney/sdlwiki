###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_CloseSensor

Close a sensor previously opened with [SDL_OpenSensor](SDL_OpenSensor)().

## Header File

Defined in [SDL_sensor.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_sensor.h), but apps should _only_ `#include <SDL3/SDL.h>`!

## Syntax

```c
void SDL_CloseSensor(SDL_Sensor *sensor);

```

## Function Parameters

|                |                                              |
| -------------- | -------------------------------------------- |
| **sensor**     | The [SDL_Sensor](SDL_Sensor) object to close |

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

