# OpenGL startup

In order for use to use OpenGL, we first need to create a context and a window
to draw in (optionally handle user inputs). Those operations ar OS specific and
OpenGL decided it will not commit for those tasks. So, we may be forced to do
those things all by ourselves. And there comes other libraries to the rescuses:

-   GLUT
-   SDL
-   SFML
-   GLFW
