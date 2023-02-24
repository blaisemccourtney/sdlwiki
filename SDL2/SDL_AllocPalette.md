###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_AllocPalette

Create a palette structure with the specified number of color entries.

## Syntax

```c
SDL_Palette* SDL_AllocPalette(int ncolors);

```

## Function Parameters

|                 |                                                             |
| --------------- | ----------------------------------------------------------- |
| **ncolors**     | represents the number of color entries in the color palette |

## Return Value

Returns a new [SDL_Palette](SDL_Palette) structure on success or NULL on
failure (e.g. if there wasn't enough memory); call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The palette entries are initialized to white.

## Version

This function is available since SDL 2.0.0.

## Related Functions

* [SDL_FreePalette](SDL_FreePalette)

----
[CategoryAPI](CategoryAPI)
