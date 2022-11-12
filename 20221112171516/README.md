# Docker layers

When creating a docker image, you provide detail instruction on which file
should be copyed and where, and which command are to be executed in order to set
up everything correcly. Doing so, in an imperative fashion, we create a stack of
operation, which results will be cached by docker in order to speed up
subsequents building. Therefore, we can optimize cache by selecting which
operation is executed first.
