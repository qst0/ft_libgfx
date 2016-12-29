### MiniLibX(3)

# MiniLibX - Managing windows

## SYNOPSYS

```C
void *
mlx_new_window ( void *mlx_ptr, int size_x, int size_y, char *title );

int
mlx_clear_window ( void *mlx_ptr, void *win_ptr );

int
mlx_destroy_window ( void *mlx_ptr, void *win_ptr );
```

## DESCRIPTION

The  `mlx_new_window()` function creates a new window on the screen, using the `size_x` and
`size_y` parameters to determine its size, and `title` as the text that should be  displayed
in  the window's title bar.

The `mlx_ptr` parameter is the connection identifier returned by
`mlx_init()` (see the [mlx man page](man_mlx.md)). `mlx_new_window()` returns a `void *`
window identifier  that  can be used by other MiniLibX calls.

Note that the MiniLibX can handle an arbitrary number of separate windows.

`mlx_clear_window()` and `mlx_destroy_window()` respectively clear (in black) and  destroy
the  given  window. They both have the same parameters: `mlx_ptr` is the screen connection
identifier, and `win_ptr` is a window identifier.

##RETURN VALUES

If `mlx_new_window()` fails to create a new window (for wathever reason), it  will  return
`NULL`, otherwise a non-null pointer is returned as a window identifier.  `mlx_clear_window`
and `mlx_destroy_window` right now return nothing.
                      
## SEE ALSO

[mlx(3)](man_mlx.md), [mlx_pixel_put(3)](man_mlx_pixel_put.md), [mlx_new_image(3)](man_mlx_new_image.md), [mlx_loop(3)](man_mlx_loop.md)

## AUTHOR

Copyright ol@ - 2002-2015 - Olivier Crouzet

### MiniLibX(3)
