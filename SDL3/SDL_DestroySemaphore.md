###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_DestroySemaphore

Destroy a semaphore.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_mutex.h), but apps should _only_ `#include <SDL3/SDL.h>`!

## Syntax

```c
void SDL_DestroySemaphore(SDL_Semaphore *sem);

```

## Function Parameters

|             |                          |
| ----------- | ------------------------ |
| **sem**     | the semaphore to destroy |

## Remarks

It is not safe to destroy a semaphore if there are threads currently
waiting on it.

## Version

This function is available since SDL 3.0.0.

## Code Examples

<<Include([SDL_CreateSemaphore](SDL_CreateSemaphore), , , from="## Begin Semaphore Example", to="## End Semaphore Example")>>

## See Also

* [SDL_CreateSemaphore](SDL_CreateSemaphore)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)


