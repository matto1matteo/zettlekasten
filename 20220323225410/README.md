# GLFW for OpenGL

To use GLFW for OpenGL, we tell it which version of OpenGL we intend to use and
which mode we want to use it

```cpp
glfwWindowHint(GLFW_CONTEXT_VERSION_MAJOR, 3);
glfwWindowHint(GLFW_CONTEXT_VERSION_MINOR, 3);
glfwWindowHint(GLFW_OPENGL_PROFILE, GLFW_OPENGL_CORE_PROFILE);
```

Extrea setup is required for MacOS.
