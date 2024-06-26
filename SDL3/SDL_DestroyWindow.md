###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_DestroyWindow

Destroy a window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h), but apps should _only_ `#include <SDL3/SDL.h>`!

## Syntax

```c
void SDL_DestroyWindow(SDL_Window *window);

```

## Function Parameters

|                |                       |
| -------------- | --------------------- |
| **window**     | the window to destroy |

## Remarks

If the window has an associated [SDL_Renderer](SDL_Renderer), it will be
implicitly destroyed as well.

If `window` is NULL, this function will return immediately after setting
the SDL error message to "Invalid window". See
[SDL_GetError](SDL_GetError)().

## Version

This function is available since SDL 3.0.0.

## See Also

* [SDL_CreatePopupWindow](SDL_CreatePopupWindow)
* [SDL_CreateWindow](SDL_CreateWindow)
* [SDL_CreateWindowWithProperties](SDL_CreateWindowWithProperties)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)


