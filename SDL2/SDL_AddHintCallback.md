###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_AddHintCallback

Add a function to watch a particular hint.

## Syntax

```c
void SDL_AddHintCallback(const char *name,
                         SDL_HintCallback callback,
                         void *userdata);

```

## Function Parameters

|                  |                                                                                                  |
| ---------------- | ------------------------------------------------------------------------------------------------ |
| **name**         | the hint to watch                                                                                |
| **callback**     | An [SDL_HintCallback](SDL_HintCallback) function that will be called when the hint value changes |
| **userdata**     | a pointer to pass to the callback function                                                       |

## Version

This function is available since SDL 2.0.0.

## Related Functions

* [SDL_DelHintCallback](SDL_DelHintCallback)

----
[CategoryAPI](CategoryAPI)
