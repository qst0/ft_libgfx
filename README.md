# ft_libgfx
42 School Graphics Custom Library

To make it easier to work with, I will be explaining and looking into the 42 School Graphics Library Minilibx.

I have uploaded all the minilibx sources for viewing and use.
[[X11]](https://github.com/qst0/ft_libgfx/tree/master/minilibx_X11_sources)
[[El Capitan]](https://github.com/qst0/ft_libgfx/tree/master/minilibx_macos_elcapitan)
[[Sierra]](https://github.com/qst0/ft_libgfx/tree/master/minilibx_macos_sierra)

Along with this goal I plan to create a set of tools and functions that can be used to make different types of programs.
The creation of these tools and functions will be set up as a series of exercises.

Basing this off my previous library for [ft_wireframe](https://github.com/qst0/ft_wireframe), [ft_fractal](https://github.com/qst0/ft_fractal) and some of the ideas going around here at the lab.

## MiniLibX

The keystone of the graphics branch at 42 is learning to use MiniLibX

Besides some old videos on intra, you are given the source and the man pages to figure it out.

To help demystify the man pages I took a moment and formatted them for markdown.

MiniLibX is described in the following man pages:

* [mlx](man_mlx.md) : MiniLibX overview
* [mlx_new_window](man_mlx_new_window.md) : manage windows
* [mlx_pixel_put](man_mlx_pixel_put.md) : draw inside window
* [mlx_new_image](man_mlx_new_image.md) : manipulate images
* [mlx_loop](man_mlx_loop.md) : handle keyboard or mouse events

Take some time and read these pages, if you want to read them in the console:

`man minilibx/man/man1/mlx.1`

The last part is the man page name, read them all.

```BASH
mlx.1
mlx_new_window.1
mlx_pixel_put.1
mlx_new_image.1
mlx_loop.1
```

I have done my best to use [markdown](https://daringfireball.net/projects/markdown/) to make a more readable experience on github.

That being said, man page formatting in the console is intresting too.

Check out [one of the man files](https://github.com/qst0/ft_libgfx/blob/master/minilibx_X11_sources/man/man3/mlx.1) to see the syntax, this one is `mlx.1`.

Once you have done that, try to open a window using the mlx functions.

If you get stuck, here is a short example:

``` C
#include <mlx.h>

int main(void)
{
  void *mlx;
  void *window;
  
  mlx = mlx_init();
  window = mlx_new_window(mlx, 1000, 1000, "Title");
  
  mlx_loop(mlx);
  return (0);
}
```

`gcc -Wall -Wextra -Werror -I minilibx -L minilibx -lmlx -framework OpenGL -framework AppKit main.c`

I certainly encourage you to figure out as much as you can with just the man pages and tinkering.

But at a certain point, you should share what you've learned and learn from others.

## More key event control - [keys.h](keys.h)

To solve the problem of knowning when many keys have been pressed I have made a struct of all the keys.

This file allows the programmer to use the minilibx loop hook to fire off events on key held.

A quick synopsis of the code:
```C
#define KEY_A 0
#define KEY_S 1
#define KEY_D 2
...

typedef struct  s_keys
{
  int           a:1;
  int           s:1;
  int           d:1;
  ...
}               t_keys
```

I really like an idea I saw on the [evil corp](https://github.com/coder-guy22296/EvilCorp) entry for the 42 Hackathon in 2016.

Where you use a constant string of all the letters to turn the keycode into it's matching printable output

It looks like this:

```
bqweryt123465=97-80]ou[ip lj\"k;\\,/nm.  ` 	. * +   / -  =012345
```

They used it to type input on to the screen along with [`mlx_string_put()`](man_mlx_pixel_put.md)

I'm sure it could be used for more! I'm thinking about making a typing game :wink:

# TODOS --- Ideas for this project when I return to it.

### TODO: STARTING POINTS

* open a window
* put a pixel on the screen
* draw a square
* draw vertical and horizonal
* [Bresenham's line algorithm](http://graphics.idav.ucdavis.edu/education/GraphicsNotes/Bresenhams-Algorithm.pdf)

### TODO: Answer Questions
What important graphics library features are missing from mlx?
Possible ideas for structures?
Possbile idea for functions?
Useful macros?

### TODO: New functions

Window management?
Safe Points Drawing?
Line Algo?

## Link Dump!
### Anything even slightly useful for coming to a better understanding of computer gfx

#### ft_wireframe
* [Ecere 3D Coding Black Hole Tutorial](http://www.ecere.com/3dbhole) :star:
* [Bresenham's Line Algorithm - Technical PDF](http://www.idav.ucdavis.edu/education/GraphicsNotes/CppNotes/Inline-Functions/CAGDNotes/Bresenhams-Algorithm.pdf)
* [Generalized Bresenham's Line Drawing Algorithm](https://www.cs.umd.edu/class/fall2003/cmsc427/bresenham.html)
* https://www.khanacademy.org/math/precalculus/precalc-matrices
* http://stackoverflow.com/questions/12554614/maths-for-color-gradient
* http://faculty.cs.tamu.edu/jchai/cpsc641_spring10/PerspectiveProjection.pdf
* http://stackoverflow.com/questions/5167269/clock-gettime-alternative-in-mac-os-x
* https://www.tutorialspoint.com/computer_graphics/visible_surface_detection.htm
* https://www.fastgraph.com/makegames/3drotation/

#### ft_fractal
* http://lodev.org/cgtutor/juliamandelbrot.html :star:
* http://www.karlsims.com/julia.html
* http://www.relativitybook.com/CoolStuff/julia_set.html
* http://paulbourke.net/fractals/apollony/
* http://www.relativitybook.com/CoolStuff/julia_set_4d.html
* http://www.fractal-animation.net/ufvp.html
* http://jonisalonen.com/2013/lets-draw-the-mandelbrot-set/
* http://stackoverflow.com/questions/33978167/julia-set-rendering-code
* http://lyc.deviantart.com/gallery/
* http://bugman123.com/index.html
* http://bugman123.com/Hypercomplex/
* https://books.google.co.uk/books?id=SJRNoOaXs2wC
* http://www.benpadiah.com/MISC_diagrams/pages/equations/holognomon.html
* http://stackoverflow.com/questions/5294955/how-to-scale-down-a-range-of-numbers-with-a-known-min-and-max-value
* http://www.toves.org/books/java/ch18-recurex/

#### wolf3d
* http://lodev.org/cgtutor/raycasting.html :star:
* [Work around lack of clock_gettime in os x](https://gist.github.com/jbenet/1087739)
* http://permadi.com/1996/05/ray-casting-tutorial-table-of-contents/
* http://mdn.github.io/canvas-raycaster/index.html

#### rt_v1
* https://www.ics.uci.edu/~gopi/CS211B/RayTracing%20tutorial.pdf

#### misc
* [Lodev's Computer Graphics Tutorials](http://lodev.org/cgtutor/) :star:
* [Javascript Graphics Tutorials](http://www.playfuljs.com/) :star:
* [OpenGL Beginners Tutorials](http://www.opengl-tutorial.org/beginners-tutorials/)
* [GSL Sandbox](http://glslsandbox.com/e#25304.0)
* [Advanced Platformer Tutorials via n++ Game Devs](http://www.metanetsoftware.com/dev/tutorials)


#### Wikipedia Links
* [Matrix mathematics](http://en.wikipedia.org/wiki/Matrix_(mathematics))
* [Orthographic_projection](https://en.wikipedia.org/wiki/Orthographic_projection)
* [Gimbal](https://en.wikipedia.org/wiki/Gimbal)
* [Gimbal lock](https://en.wikipedia.org/wiki/Gimbal_lock)
* [Ray casting](https://en.wikipedia.org/wiki/Ray_casting)
* [Bresenham's line algorithm](https://en.wikipedia.org/wiki/Bresenham%27s_line_algorithm)
* [Sierpinski carpet](https://en.wikipedia.org/wiki/Sierpinski_carpet)
* [Apollonian gasket](https://en.wikipedia.org/wiki/Apollonian_gasket)
* [Julia set](https://en.wikipedia.org/wiki/Julia_set)
