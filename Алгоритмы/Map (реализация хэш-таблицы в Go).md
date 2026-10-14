```go
package main

  

import "fmt"

  

func main() {

    friends := make(map[string][]string)

  

    friends["бобик"] = []string{"ваня", "катя"}

    friends["ваня"] = []string{"бобик", "катя"}

    friends["катя"] = []string{"бобик", "ваня"}

  

    fmt.Println(friends)

}
```
