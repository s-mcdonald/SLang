## Control Flow


#### if
```c

    if (n == 0) 
    {
        return 1;
    } 
    
    if ( n == 0 ) 
    {
        return 1;
    } 
    else if (n > 5)
    {
        return n / 5;
    }

```


#### for
```c

    array bag = [1, 5, 7, 9, 33, 55, 88];
    
    for (item in bag)
    {
        terminal item;
    } 
    
    
    for ( i, v in bag)
    {
        terminal "The index is  : " concat i;
        terminal "The value is  : " concat v;
    } 

```

#### until
```c
    
    until (x >= 55)
    {
        // do something
        x++;
    } 
    
```
