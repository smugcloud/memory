# Variable Memory Allocation

This is a helper library to quickly determine the total memory allocation of a variable.  This includes the space occupied by the type, plus the contents of the variable.  

Currently supported types:
```
string
slice
map
struct
```

## Example
```
package main

import (
    "fmt"
    "github.com/smugcloud/memory"
)

func main(){
    s := "example"
    fmt.Println(memory.GetSize(s))
}
```