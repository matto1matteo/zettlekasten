# OpenGL object

OpenGL is a C library, thus can't use abstractions of the OOP world. Instead, it
defines "object" in a fancy way. Those objects are struct, collections of
options, that represents a subset of the OpenGL's context.

```c
struct object_name {
    float  option1;
    int    option2;
    char[] name;
};

// The State of OpenGL
struct OpenGL_Context {
  	...
  	object_name* object_Window_Target;
  	...  	
};

// create object
unsigned int objectId = 0;
glGenObject(1, &objectId);
// bind/assign object to context
glBindObject(GL_WINDOW_TARGET, objectId);
// set options of object currently bound to GL_WINDOW_TARGET
glSetObjectOption(GL_WINDOW_TARGET, GL_OPTION_WINDOW_WIDTH,  800);
glSetObjectOption(GL_WINDOW_TARGET, GL_OPTION_WINDOW_HEIGHT, 600);
// set context target back to default
glBindObject(GL_WINDOW_TARGET, 0);
```

We create an object by assign it an id, then, to use it, we bind it to a context
and set the options. In the end, we can turn back to bind the original object
(in this case to the context).
