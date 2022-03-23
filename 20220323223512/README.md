# GLAD

Since there are many different version of OpenGL for every manufacturer driver,
we need to be able to specify which version we want to take in account and this
must be done at run-time. So, it's our task to retrieve the location of the
desired function. This is OS-specific, though, we can utilize helpfull libraries
such as [GLAD](https://glad.dav1d.de/), which comes to us as a web service that
generates required headers and source.
