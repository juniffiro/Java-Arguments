# Basic Java Flags
Can be used to optimize a server or program.

# Memory allocation

| Flag | Description                       |
|------|-----------------------------------|
 | -Xms | Minimum allocated memory for Heap |
 | -Xmx | Maximum allocated memory for Heap |
 | -Xss | Allocated memory for Stack        |

# Main flags

| Flag                             | Description                                                                                                                                     | Note              |
|----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|
| -XX:+DisableAttachMechanism      | Disable the attachment mechanism that allows agents to be loaded into the JVM                                                                   |                   |
| -Xincgc                          | Activates the garbage collector, which will unload unused RAM from time to time. The collector type is chosen depending on the version of Java. |                   |
| -server                          | Java server activation. Speeds up the compilation of classes, which gives a performance boost, but increases the startup time.                  | Only for Java x64 |
| -Dfile.encoding=UTF-8            | UTF-8 encoding                                                                                                                                  |                   |
| -XX:AutoGCSelectPauseMillis=3000 | The time in milliseconds between calls to the automatically selected garbage collector.                                                         |                   |
| -XX:+UseConcMarkSweepGC          | Activating a garbage collector that uses multiple threads                                                                                       |                   |
| -XX:ConcGCThreads=2              | Number of threads for garbage collector                                                                                                         |                   |
| -XX:+UseSerialGC                 | Garbage collector that runs on a single thread                                                                                                  |                   |

# Additional for optimization

| Flag                      | Description                                                                               | Note |
|---------------------------|-------------------------------------------------------------------------------------------|------|
| -XX:+AggresiveOpts        | Activating Java Experimental Arguments                                                    |      |
| -XX:-UseGCOverheadLimit   | Ignores low memory for garbage collection                                                 |      |
| -XX:+UseCompressedOops    | Reducing the size of the pointer, headings, as well as shifts within the created objects. |      |
| -XX:+OptimizeFill         | Allows you to translate array fill/copy cycles into direct machine instructions.          |      |
| -XX:+OptimizeStringConcat | Optimization of the concatenation operation.                                              |      |