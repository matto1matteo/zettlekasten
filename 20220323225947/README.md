# Create a Window with OpenGL

Once GLFW is correctly condifured, it's quite easy to create a window:

```cpp
//                                  with  heigth title            who knows??
GLFWwindow* window = glfwCreateWindow(800, 600, "Title goes here", NULL, NULL);
if (window == NULL)
{
    std::cout << "Failed to create GLFW window" << std::endl;
    glfwTerminate();
    return -1;
}
glfwMakeContextCurrent(window);
```

The window object will be used as main context for the current thread.
