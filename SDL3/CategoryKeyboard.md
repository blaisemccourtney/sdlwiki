
# Keyboard Support

'''Include File(s):'''  [http://hg.libsdl.org/SDL/file/default/include/SDL_keyboard.h SDL_keyboard.h], [http://hg.libsdl.org/SDL/file/default/include/SDL_keycode.h SDL_keycode.h], [http://hg.libsdl.org/SDL/file/default/include/SDL_scancode.h SDL_scancode.h]



## Introduction

This category contains functions for handling keyboard inputs.  

SDL uses two different types of values to represent keys on the keyboard - scancode and keycode.

[[SDL_Scancode]] values are used to represent the physical location of a keyboard key on the keyboard. Values of this type are used to represent keyboard keys in the <code>key.keysym.scancode</code> field of the [[SDL_Event]] structure, among other places. The values in the [[SDL_Scancode]] enumeration are based on the USB usage page standard (http://www.usb.org/developers/docs/).  Scancode constants use the symbol name prefixed with SDL_SCANCODE_ (eg: SDL_SCANCODE_SPACE). 

[[SDL_Keycode]] values are mapped to the current layout of the keyboard and correlate to an [[SDL_Scancode]]. Values of this type are used to represent key symbols in the <code>key.keysym.sym</code> field of the [[SDL_Event]] structure, among other places. The values in the [[SDL_Keycode]] enumeration are based on Unicode values representing the unmodified character that would be generated by pressing the key, or the scancode value with the high bit set (bitwise ORed with 0x40000000) for those keys that do not generate characters.  Keycode constants use the symbol name (lowercased for letters) prefixed with SDLK_ (eg: SDLK_SPACE).<br/>
A special exception is the number keys at the top of the keyboard which always map to SDLK_0, SDLK_1, ..., SDLK_9, regardless of layout.

The main difference between these two values comes into play in situations where the operating system is mapping the physical keyboard keys to different virtual letters. For instance, when a standard QWERTY keyboard is mapped to a German QWERTZ layout, the "Y" key will generate events with a scancode of SDL_SCANCODE_Y, but a keycode of SDLK_z. Which one to use is left to the application: scancodes are suited in situations where controls are layout-dependent (eg. the "WASD" keys as left-handed arrow keys), whereas keycodes are better suited to situations where controls are character-dependent (eg. the "I" key for '''I'''nventory).

## Enumerations
<<FullSearchCached(category:CategoryEnum CategoryKeyboard -title:SGEnumerations)>>

## Structures
<<FullSearchCached(category:CategoryStruct CategoryKeyboard -title:SGStructures)>>

## Functions
<<FullSearchCached(category:CategoryKeyboard -CategoryEnum -CategoryStruct -title:SGFunctions)>>

<!-- BEGIN CATEGORY LIST -->
- [SDL_Keycode](SDL_Keycode)
- [SDL_Keymod](SDL_Keymod)
- [SDL_Keysym](SDL_Keysym)
- [SDL_Scancode](SDL_Scancode)
<!-- END CATEGORY LIST -->
----
CategoryCategory