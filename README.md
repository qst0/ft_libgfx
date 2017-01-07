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

*This is on hold for the moment, so I can get the remaining experience to join the PHP piscine.*

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
* http://www.ecere.com/3dbhole/mathematics_of_3d_graphics.html
* http://www.ecere.com/3dbhole/3d_transformations.html
* http://www.idav.ucdavis.edu/education/GraphicsNotes/CppNotes/Inline-Functions/CAGDNotes/Bresenhams-Algorithm.pdf
* https://www.cs.umd.edu/class/fall2003/cmsc427/bresenham.html
* https://www.khanacademy.org/math/precalculus/precalc-matrices
* http://stackoverflow.com/questions/12554614/maths-for-color-gradient
* http://faculty.cs.tamu.edu/jchai/cpsc641_spring10/PerspectiveProjection.pdf
* https://gist.github.com/jbenet/1087739
* http://stackoverflow.com/questions/5167269/clock-gettime-alternative-in-mac-os-x
* https://www.tutorialspoint.com/computer_graphics/visible_surface_detection.htm
* https://www.fastgraph.com/makegames/3drotation/

#### ft_fractal
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

#### wolf3d
* http://permadi.com/1996/05/ray-casting-tutorial-table-of-contents/
* http://mdn.github.io/canvas-raycaster/index.html
* http://www.toves.org/books/java/ch18-recurex/

#### rt_v1
* https://www.ics.uci.edu/~gopi/CS211B/RayTracing%20tutorial.pdf

#### misc
* http://lodev.org/cgtutor/
* http://www.opengl-tutorial.org/beginners-tutorials/
* http://glslsandbox.com/e#25304.0


#### Wikipedia Links
* http://en.wikipedia.org/wiki/Matrix_(mathematics)
* https://en.wikipedia.org/wiki/Orthographic_projection
* https://en.wikipedia.org/wiki/Gimbal
* https://en.wikipedia.org/wiki/Gimbal_lock
* https://en.wikipedia.org/wiki/Ray_casting
* https://en.wikipedia.org/wiki/Bresenham%27s_line_algorithm
* https://en.wikipedia.org/wiki/Sierpinski_carpet
* https://en.wikipedia.org/wiki/Apollonian_gasket
* https://en.wikipedia.org/wiki/Julia_set
