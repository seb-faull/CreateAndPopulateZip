# Create and Populate a Zip File System

This is a small project I have created to play around with creating a file system and reading and writing files to it.

## Summary

### java.io.package
- Stream-based I/O
- Legacy file/filesystem types

Those were the streams that were very tied to files themselves. We don't want to use those in our new code, but you want to be aware of them because there is still a lot of code out there that uses them.

### java.nio.file.package
- File/filesystem types

### Streams
- Ordered sequence of data
- Unidirectional: either for reading from or writing to
- Binary (data oriented) or character based (unicode oriented)
    - Working with them tends to be very much the same, they pretty much have the same operations, they just interact with the content at different levels.

- Can be chained together

### Try-with-resources
- Automates resource cleanup
- Resources implement AutoCloseable

### Key Types

#### Path
- Locates a file system item
- Includes the file system

#### Paths (convenience class)
- Factory for Path instances for default file system

### Files
- Methods for interacting with files

### FileSystem
- Represents a file system (defaults file system)
- Can have specialised file system such as .zip
- File systems are identified by URIs
    - For example the ZIP file system is represented by URIs with the scheme "jar:file"

### FileSystems
- Methods to create/open file system
