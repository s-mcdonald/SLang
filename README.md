# SLang (programming language)

`S` lang pronounced _'slang'_, is a minimalist programming language designed to compile directly to machine code. It is purpose-built to create simple, maintainable systems with a focus on readability, easy debugging, and long-term maintainability.

### 🚧 SLang is Under Development 🚧

### Core Goals
* **Ease of Learning**: Even simpler than Lua.
* **Fast Compilation**: Prioritizes blazing-fast compilation times.
* **Automatic Memory Management**: Includes built-in garbage collection.
* **Direct Compilation**: Compiles directly to machine code.


This is a little bit of fun, but I set out to achieve a small, fast real-life usable language.

Below is essentially a compilable program. Note that there is no main function; 
we define an entry point by the name of the file `slang.s` A return value
is optionally returned at the end of the file otherwise 0 is implied.


#### File: slang.s
```c++
    terminal "Hello World..";
```

#### Infer types at compile time.

```c++

    so x = 5;        ;; int
    so y = 50 / 9;   ;; float
    
```


#### Auto Deferred triggers

```c++

    y = 1;
    x = 4;

    when (x == 5) [y] { //< we capture by value at time on instantiation
        // we have reference to y while it is value of 1
        printf("result is: %s", x + y);
    }
        
    y = 7;
    x = 5; // now the above code triggers

    // result is: 6
    
```