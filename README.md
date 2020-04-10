# ft_libgfx AKA b_gfx overload

## NEWS UPDATE: New Projects Coming!

> Hello everyone, hope you are staying safe. We have new projects coming with the new cursus in 2020. The information here should stay relevant but I look forward to updating it when we get the new subjects.

Greetings b_gfx'rs and hackers alike!
For your reading pleasure, [dark-mode is on github-pages](https://qst0.github.io/ft_libgfx/).

#### To make it easier to work with, I will be explaining and looking into the 42 School Graphics Library Minilibx.

Oh wait what is this?
[![Hexcross by MetaHobby, vine board with timed game](https://metahobby.com/wp-content/uploads/2019/04/Simulator-Screen-Shot-iPhone-8-Plus-2019-04-13-at-02.54.57.png)](https://play.google.com/store/apps/details?id=com.metahobby.hexcross&utm_source=ft_libgfx)

Oh! It's a shameless plug for my latest video game: [Hexcross](https://play.google.com/store/apps/details?id=com.metahobby.hexcross&utm_source=ft_libgfx)

I've been back working in this type of project now (escaping from web, database and other duties) so look forward to more screen shots and juice knowledge as I find it. Probably a refactor of this resource at some point too...

[![metaHobbyLogo](https://metahobby.com/wp-content/uploads/2019/06/spr_credits_qst.png)](https://metahobby.com/beta)

[Want to beta test our upcoming game?](https://metahobby.com/beta)


Without futher ado:

#### To make it easier to work with, I will be explaining and looking into the 42 School Graphics Library Minilibx.

I have uploaded all the minilibx sources for viewing and use.
[[X11]](https://github.com/qst0/ft_libgfx/tree/master/minilibx_X11_sources)
[[El Capitan]](https://github.com/qst0/ft_libgfx/tree/master/minilibx_macos_elcapitan)
[[Sierra]](https://github.com/qst0/ft_libgfx/tree/master/minilibx_macos_sierra)

Along with this goal I plan to create a set of resources and functions that can be used to make different types of computer graphics programs. The resources will be aimed at helping others create great 42 graphics projects and encouraging graphics [side projects](https://github.com/all-hack/42moonlight).

#### Contents:

* [The Graphics Branch](#the-graphics-branch)
* [Graphics Branch Link Dump](#graphics-branch-link-dump)
* [MiniLibX](#minilibx)
* [Getting started with fdf (ft_wireframe)](#getting-started-with-fdf-ft_wireframe)
* [Getting started with fractol ft_fractal](#getting-started-with-fractol-ft_fractal)
* [More key event control - keys.h](#more-key-event-control---keysh)
* [What about events?](#what-about-events)
* [TODOS](#todos)

Email me at `msnyng+gfx`@`gmail.com` with any questions you might have about this repo.

If you are at 42, please reach out to qst0 in person for questions.
They are best that way. Currently in 42 Accelerate in Zone 4.

Please feel free to fork or contribute to this repo. It would look good, right? 

Not at 42? Following the graphics projects somewhere else? Just curious?

This repo still has treasures for you,
please check out the [link dump](#graphics-branch-link-dump).

## The Graphics Branch

The goals of the graphics branch projects can be put simply:

* Rasterisation, show a wireframe from a file
* Render trippy colored mandelbrot and julia set
* Create a ray caster game engine like wolfenstein
* Build a 'first try' ray tracer
* Work with a team to build a feature rich ray tracer

Let's get started.

# Graphics Branch Link Dump
### Anything even slightly useful for coming to a better understanding of gfx

* [Learn Computer Graphics From Scratchapixel.com](https://www.scratchapixel.com/) :star:
* [MLX Cookbook Post 42Network](https://stackoverflow.com/c/42network/questions/164)

#### ft_wireframe
* [Ecere 3D Coding Black Hole Tutorial](http://www.ecere.com/3dbhole) :star:
* [Bresenham's Line Algorithm - Technical PDF](http://www.idav.ucdavis.edu/education/GraphicsNotes/CppNotes/Inline-Functions/CAGDNotes/Bresenhams-Algorithm.pdf)
* [Generalized Bresenham's Line Drawing Algorithm](https://www.cs.umd.edu/class/fall2003/cmsc427/bresenham.html)
* [Perspective Projection PDF](http://faculty.cs.tamu.edu/jchai/cpsc641_spring10/PerspectiveProjection.pdf)
* [Math for color gradient](http://stackoverflow.com/questions/12554614/maths-for-color-gradient)
* [Visible surface detection](https://www.tutorialspoint.com/computer_graphics/visible_surface_detection.htm)
* [3D Rotation](https://www.fastgraph.com/makegames/3drotation/)
* [Khanacademy Precalc Matrices](https://www.khanacademy.org/math/precalculus/precalc-matrices)

#### ft_fractal
* [Lodev Julia and Mandelbrot Tutorial](http://lodev.org/cgtutor/juliamandelbrot.html) :star:
* [Plot the Mandelbrot Set by Hand](http://www.wikihow.com/Plot-the-Mandelbrot-Set-By-Hand)
* [Real-time animated fractal in only 32 lines of Javascript code](http://slicker.me/fractals/animate.htm)
* [Understanding Julia and Mandelbrot Sets - Karl Sims](http://www.karlsims.com/julia.html)
* [Alt.fractals - Cool Stuff: Fractals](http://www.relativitybook.com/CoolStuff/julia_set.html)
* [Apollony Fractal - written by Paul Bourke](http://paulbourke.net/fractals/apollony/)
* [Alt.fractals - Cool Stuff: 4d Julia](http://www.relativitybook.com/CoolStuff/julia_set_4d.html)
* [the   Ultimate   Fractal   Video   Project   !](http://www.fractal-animation.net/ufvp.html)
* [Mandelbrot set tutorial](http://jonisalonen.com/2013/lets-draw-the-mandelbrot-set/)
* [Julia set rendering code](http://stackoverflow.com/questions/33978167/julia-set-rendering-code)
* [Fractal inspiration via Lyc on Deviantart](http://lyc.deviantart.com/gallery/)
* [Hypercomplex Fractals](http://bugman123.com/Hypercomplex/)
* [Alt.fractals: A Visual Guide to Fractal Geometry and Design](https://books.google.co.uk/books?id=SJRNoOaXs2wC)
* [Infinite division of congruent similarities](http://www.benpadiah.com/MISC_diagrams/pages/equations/holognomon.html)
* [Scale a range to a known min and max](http://stackoverflow.com/questions/5294955/how-to-scale-down-a-range-of-numbers-with-a-known-min-and-max-value)
* [Java recursion examples](http://www.toves.org/books/java/ch18-recurex/)


#### wolf3d
* [Lodev Raycasting Tutorial](http://lodev.org/cgtutor/raycasting.html) :star:
* [Raycasting Tutorial (Theory)](http://permadi.com/1996/05/ray-casting-tutorial-table-of-contents/)
* [Stackoverflow question: clock_gettime](http://stackoverflow.com/questions/5167269/clock-gettime-alternative-in-mac-os-x)
* [Code for clock_gettime alternative in os x](https://gist.github.com/jbenet/1087739)
* [JS Raycaster Tutorial](http://www.playfuljs.com/a-first-person-engine-in-265-lines/)
* [Canvas Raycaster](http://mdn.github.io/canvas-raycaster/index.html)
* [Raycast Height Maps Example](http://simulationcorner.net/index.php?page=comanche)
* [EXTRA: John Carmack: Systems Engineering Technical Talk](https://www.youtube.com/watch?v=lHLpKzUxjGk) :star:

#### rt_v1
* [Codermind team Ray Tracing Tutorial PDF](https://sebastiandang.github.io/docs/cse168/RayTracing.pdf)
* [UC Davis Lecture : 49 minutes](https://www.youtube.com/watch?v=Ahp6LDQnK4Y)
* [Disney's Practical Guide to Path Tracing : 10 minutes](https://www.youtube.com/watch?v=frLwRLS_ZR0)

#### misc
* [Lodev's Computer Graphics Tutorials](http://lodev.org/cgtutor/) :star:
* [Javascript Graphics Tutorials](http://www.playfuljs.com/) :star:
* [OpenGL Beginners Tutorials](http://www.opengl-tutorial.org/beginners-tutorials/)
* [GSL Sandbox](http://glslsandbox.com/e#25304.0)
* [Advanced Platformer Tutorials via n++ Game Devs](http://www.metanetsoftware.com/dev/tutorials)
* [Haxiomic GPU Fluid Experiments](http://haxiomic.github.io/GPU-Fluid-Experiments/html5/)
* [Bugman123](http://bugman123.com/index.html)


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

## MiniLibX

The keystone of the 42 graphics branch is learning to use MiniLibX

Besides some [old videos on intra](https://elearning.intra.42.fr/notions/fdf/subnotions), you are given the source and the man pages to figure it out.

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

Remember, where this line above says `minilibx` yours might say something like `minilibx_macos_sierra` it's simply the name of the folder with mlx built in it. Speaking of which, be sure to build mlx like so: `cd <mlxfolder>` `make`

I certainly encourage you to figure out as much as you can with just the man pages and tinkering.

But at a certain point, you should show what you've learned and learn from others.

## Getting started with fdf [(ft_wireframe)](https://github.com/qst0/ft_wireframe)

Well first of all, check out all the [juicy details](https://projects.intra.42.fr/fdf/mine) they give us.

It's a solid set of guidelines but nowhere to start. *42 Classic*. But it won't be like this the whole way.
Since the system is set up this way I would highly recommend experementing with any ideas you have right now.
Get comfortable trying to make something happen, use events, loops and anything else you found in the man pages.

Once you have done this, you should already be thinking about:

[Bresenham's line algorithm](http://graphics.idav.ucdavis.edu/education/GraphicsNotes/Bresenhams-Algorithm.pdf)

Drawing a line, various curves and shapes are normally handled by a graphics library. At 42 we will doing all of this from scratch, minilibx is not feature rich for *some reason*. Since we are rendering a grid, that line algorithm is where we need to start. The link above is to a very detailed proof of the algorithm. In the links below you can find more on the subject. 

That's all for now, find me if you have any more questions or suggestions for the fdf section.

*This part of the guide is a work in progress, ask if you have a question for now*

There are more resources, examples and inspiration [in the link dump].(#graphics-branch-link-dump)

## Getting started with fractol [(ft_fractal)](https://github.com/qst0/ft_wireframe)

There are many good resources on this adventure in computer graphics, but I would argue the best place to start is on paper.

Look up imaginary numbers. Throw some numbers into the function for the mandelbrot.

`f(x) = z² + c`

Real numbers, imaginary numbers then complex numbers.
[Here is a guide](http://www.wikihow.com/Plot-the-Mandelbrot-Set-By-Hand)

It would seem to me the key to this project, like any other, is to get hands on and experement.

Here is a macro for formula that might be useful:

[Scale a range to a known min and max](http://stackoverflow.com/questions/5294955/how-to-scale-down-a-range-of-numbers-with-a-known-min-and-max-value)

```C
#define RANGE_CHANGE(x,a,b,min,max) (((b)-(a))*((x)-(min))/((max)-(min)))+(a)
```

*This part of the guide is a work in progress, ask if you have a question for now*

There are more resources, examples and inspiration [in the link dump].(#graphics-branch-link-dump)

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

## What about events?

It's a good idea to experement with the events they mention in the man pages, but there is more than that!

Check out the [mlx_loop](man_mlx_loop.md) man page, at the bottom is says to look at [mlx_int_param_event.c](https://github.com/qst0/ft_libgfx/blob/master/minilibx_X11_sources/mlx_int_param_event.c)

In this code we can see:

```C
int	(*(mlx_int_param_event[]))() =
{
  mlx_int_param_undef,   /* 0 */
  mlx_int_param_undef,
  mlx_int_param_KeyPress,
  mlx_int_param_KeyRelease,  /* 3 */
  mlx_int_param_ButtonPress,
  mlx_int_param_ButtonRelease,
  mlx_int_param_MotionNotify,  /* 6 */
  ...
```

This can help you make sense of the command `mlx_hook` in [mlx_hook.c](https://github.com/qst0/ft_libgfx/blob/master/minilibx_X11_sources/mlx_hook.c)

We can create our own key hooks with this information:

```C
void	set_hooks(t_view *v)
{
	mlx_do_key_autorepeatoff(v->mlx);
	mlx_hook(v->window, 2, 0, key_press_hook, v);
	mlx_hook(v->window, 3, 0, key_release_hook, v);
	mlx_hook(v->window, 4, 0, mouse_press_hook, v);
	mlx_hook(v->window, 5, 0, mouse_release_hook, v);
	mlx_hook(v->window, 6, 0, motion_hook, v);
	mlx_hook(v->window, 12, 0, expose_hook, v);
	mlx_hook(v->window, 17, 0, exit_hook, v);
}
```

The example above shows all the useful hook params I have found, please help me find any more!

The exit_hook (which you could name anything) is the undocumented magic to take from this code.

It's how you can stop your program with the `exit(0);` command when the user presses the closing button on the window.

# TODOS
#### Progress Goals for the Project

### TODO: MORE LINKS!

`(I have more links I need to add and sort! CHECK FOR DUPLICATES!)`

https://en.wikipedia.org/wiki/Linear_interpolation

https://en.wikipedia.org/wiki/X_PixMap

https://en.wikipedia.org/wiki/BMP_file_format

https://www.cs.uic.edu/~jbell/CourseNotes/ComputerGraphics/3DTransforms.html

https://www.online-utility.org/image/convert/to/XMP

https://open.gl/transformations

https://en.wikipedia.org/wiki/Lissajous_curve

https://randomascii.wordpress.com/2011/08/13/faster-fractals-through-algebra/

http://softpixel.com/~cwright/programming/threads/threads.c.php

https://en.wikipedia.org/wiki/Parallax

https://www.youtube.com/watch?v=HQYsFshbkYw

https://en.wikipedia.org/wiki/Digital_differential_analyzer_(graphics_algorithm)

https://github.com/shaunlebron/blinky

http://bisqwit.iki.fi/jutut/kuvat/programming_examples/portalrendering.html

### TODO: STARTING POINTS EXPLAINED

* put a pixel on the screen
* draw particles on the screen
* draw vertical and horizonal lines
* draw a square / circle / triangle

### TODO: Answer Questions

What important graphics library features are missing from mlx?

* Many things are missing from mlx, drawing, rotating, redraw and all sorts of events

Possible ideas for structures?

* We could use something that could store the data in a point
* Try to make something that can hold you mlx pointer and window to pass to the loop hook

Possbile idea for functions?

* Make a function that puts a pixel into an mlx image

Useful macros?

* Be sure to set constants as macros, move any global variables into a structure

What about window management?

* I don't know of any way to move the window or place it in another area in mlx.
