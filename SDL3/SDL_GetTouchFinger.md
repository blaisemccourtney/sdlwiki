###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)

## Draft

**THIS PAGE IS A WORK IN PROGRESS** ... Please make edits to this page to improve it!



<!-- #*^*^*^*^*See https://wiki.libsdl.org/SGFunctions for details on editing this page*^*^*^*^* -->
# SDL_GetTouchFinger

Get the finger object for specified touch device ID and finger index.

## Header File

Defined in [SDL_touch.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_touch.h), but apps should _only_ `#include <SDL3/SDL.h>`!

## Syntax

```c
SDL_Finger * SDL_GetTouchFinger(SDL_TouchID touchID, int index);

```

## Function Parameters

|                 |                                      |
| --------------- | ------------------------------------ |
| **touchID**     | the ID of the requested touch device |
| **index**       | the index of the requested finger    |

## Return Value

Returns a pointer to the [SDL_Finger](SDL_Finger) object or NULL if no
object at the given ID and index could be found.

## Remarks

The returned resource is owned by SDL and should not be deallocated.

## Version

This function is available since SDL 3.0.0.

## See Also

* [SDL_GetNumTouchFingers](SDL_GetNumTouchFingers)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryEvents](CategoryEvents), [CategoryDraft](CategoryDraft)
<!-- #See the Style Guide for instructions on editing the footer. -->


