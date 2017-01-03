### MiniLibX(3)

# MiniLibX - Simple Graphical Interface Library for students

## SYNOPSYS

```C
#include  <mlx.h>

void  *
mlx_init();
```

## DESCRIPTION

MiniLibX is an easy way to create graphical software, without any X-Window/Cocoa programming knowledge.
It provides simple window creation, a drawing tool, image and basic events management.

## BSD/LINUX X-WINDOW CONCEPT

X-Window  is a network-oriented graphical system for Unix. It is based on two main parts: 

On one side, your software wants to draw something on the screen and/or get keyboard & mouse entries.

On the other side, the X-Server manages the screen, keyboard and mouse (It is often refered to as a "display").

A network connection must be established between these two entities  to send  drawing  orders
(from  the  software  to the X-Server), and keyboard/mouse events (from the X-Server to the software).

## MACOS CONCEPT
The MacOSX operating system handle graphical access to the  screen (or "display").

On one side, your software wants to draw something on the screen and/or get keyboard & mouse entries.

On the other side, the underlying MacOSX graphical framework that  handles the screen, the windowing system, keyboard and mouse.

A connection between these two entities must be established.

## INCLUDE FILE

`mlx.h` should be included for a correct use of the MiniLibX API.

It only contains function prototypes, no structure is needed.

## LIBRARY FUNCTIONS

First of all, you need to initialize the connection between your  software  and  the display.

Once this connection is established, you'll be able to use other MiniLibX functions to send the graphical orders,
like "I  want  to draw a yellow pixel in this window" or "did the user hit a key?".

The `mlx_init()` function will create this connection.
No  parameters  are needed, and it will return a void* identifier, used for further calls to the library routines.

All other MiniLibX functions are described in the following man pages:

* [mlx_new_window](man_mlx_new_window.md) : manage windows

* [mlx_pixel_put](man_mlx_pixel_put.md) : draw inside window

* [mlx_new_image](man_mlx_new_image.md) : manipulate images

* [mlx_loop](man_mlx_loop.md) : handle keyboard or mouse events

LINKING MinilibX on BSD/Linux and X-Window
To use MiniLibX functions, you'll need to link your software with
several  libraries,  including  the  MiniLibX library itself.  To do this,
simply add the following arguments at linking time:
       
`-lmlx -lXext -lX11`

You may also need to specify the path to these libraries, using the `-L` flag.


## LINKING Minilibx on MACOSX

To  use  MiniLibX functions, you'll need to link your software with the MiniLibX library, and several system frameworks:

`-lmlx -framework OpenGL -framework AppKit`

You may also need to specify the path to the MiniLibX library, using the `-L` flag.

## RETURN VALUES

If `mlx_init()` fails to set up the connection to the graphical system, it will return NULL,
otherwise a non-null pointer is returned as a connection identifier.

## SEE ALSO

[mlx_new_window(3)](man_mlx_new_window.md), [mlx_pixel_put(3)](man_mlx_pixel_put.md),
[mlx_new_image(3)](man_mlx_new_image.md), [mlx_loop(3)](man_mlx_loop.md)

## AUTHOR

Copyright ol@ - 2002-2015 - Olivier Crouzet

### MiniLibX(3)
