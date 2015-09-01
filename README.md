# MapReduce_StringMatch
Improved the original mars with atomic operation.
When the original authors were working on the project, the atomic
operation was not supported on GPUs, so they had to come up with 2 step
approach (step 1 to calculate the size to allocate in GPUs step 2 to
actually call map/reduce function.) When we were working on improving
the performance of Mars, atomic operations are supported. We just need
to do minor changes mainly in the MarLib.cu and main.cu files.

automic operation in C++
http://blog.csdn.net/yockie/article/details/8838686
