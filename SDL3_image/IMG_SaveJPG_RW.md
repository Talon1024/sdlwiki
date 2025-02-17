###### (This function is part of SDL_image, a separate library from SDL.)
# IMG_SaveJPG_RW

Save an SDL_Surface into JPEG image data, via an SDL_RWops.

## Syntax

```c
int IMG_SaveJPG_RW(SDL_Surface *surface, SDL_RWops *dst, int freedst, int quality);

```

## Function Parameters

|                 |                                                                                    |
| --------------- | ---------------------------------------------------------------------------------- |
| **freedst**     | SDL_TRUE to close/free the SDL_RWops before returning, SDL_FALSE to leave it open. |
| **surface**     | the SDL surface to save                                                            |
| **dst**         | the SDL_RWops to save the image data to.                                           |
| **freedst**     | SDL_TRUE to close/free the SDL_RWops before returning, SDL_FALSE to leave it open. |

## Return Value

Returns 0 if successful, -1 on error.

## Remarks

If you just want to save to a filename, you can use
[IMG_SaveJPG](IMG_SaveJPG)() instead.

## Version

This function is available since SDL_image 3.0.0.

## Related Functions

* [IMG_SaveJPG](IMG_SaveJPG)

----
[CategoryAPI](CategoryAPI)

