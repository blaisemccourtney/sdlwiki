###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_GetDesktopDisplayMode

Get information about the desktop's display mode.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h), but apps should _only_ `#include <SDL3/SDL.h>`!

## Syntax

```c
const SDL_DisplayMode* SDL_GetDesktopDisplayMode(SDL_DisplayID displayID);

```

## Function Parameters

|                   |                                         |
| ----------------- | --------------------------------------- |
| **displayID**     | the instance ID of the display to query |

## Return Value

Returns a pointer to the desktop display mode or NULL on error; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

There's a difference between this function and
[SDL_GetCurrentDisplayMode](SDL_GetCurrentDisplayMode)() when SDL runs
fullscreen and has changed the resolution. In that case this function will
return the previous native display mode, and not the current display mode.

## Version

This function is available since SDL 3.0.0.

## Code Examples

```c++
SDL_DisplayMode dm;
if (SDL_GetDesktopDisplayMode(0, &dm) != 0) {
    SDL_Log("SDL_GetDesktopDisplayMode failed: %s", SDL_GetError());
    return 1;
}
```

## See Also

* [SDL_GetCurrentDisplayMode](SDL_GetCurrentDisplayMode)
* [SDL_GetDisplays](SDL_GetDisplays)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)


