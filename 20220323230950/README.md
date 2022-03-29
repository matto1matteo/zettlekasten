# Set up GLAD

Set up GLAD loader to call OpenGL functions

```cpp
if (!gladLoadGLLoader((GLADloadproc)glfwGetProcAddress))
{
    std::cout << "Failed to initialize GLAD" << std::endl;
    return -1;
}
```

We pass GLAD the function to load the address of the OpenGL function pointers
which is OS-specific. GLFW gives us `glfwGetProcAddress` that defines the
correct function based on which OS we're compiling for.
