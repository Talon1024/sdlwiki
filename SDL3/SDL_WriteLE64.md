###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_WriteLE64

Use this function to write 64 bits in native format to a [SDL_RWops](SDL_RWops) as little-endian data.

## Syntax

```c
size_t SDL_WriteLE64(SDL_RWops * dst, Uint64 value);

```

## Function Parameters

|               |                                          |
| ------------- | ---------------------------------------- |
| **dst**       | the stream to which data will be written |
| **value**     | the data to be written, in native format |

## Return Value

Returns 1 on successful write, 0 on error.

## Remarks

SDL byteswaps the data only if necessary, so the application always
specifies native format, and the data written will be in little-endian
format.

## Version

This function is available since SDL 3.0.0.

## Related Functions

* [SDL_WriteBE64](SDL_WriteBE64)

----
[CategoryAPI](CategoryAPI), [CategoryIO](CategoryIO)


