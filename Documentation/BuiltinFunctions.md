## Core Functions

__INDEX__

```
#### files(str: path)               -> list of files as string
#### read(str: filename)            -> string of text from file
#### copy(str: path, str: path2)    -> copy file from and to.
#### compress(str: filename, )      -> compress files to single zip
#### decompress()                   -> extract a compressed file
```

#### Read a text file
```c
string contents = read("/path/to/file");
```

#### Copy a file to another location
```c
bool success = copy("/path/to/file", "/path/to/newfilename");
```


#### Compress a file or folder
```c
bool success = compress("filename.zip", files("/path/to/fodler"));
bool success = compress("filename.zip", [
            "/path/to/file1",
            "/path/to/file2",
            "/path/to/file3",
        ],
    );
```

#### DeCompress a file
```c
bool success = decompress("/path/to/file.zip", "/path/to/extract/to/extract");
```
