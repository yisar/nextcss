# cssnext
Postcss alternative.

### [Playground](https://yisar.github.io/cssnext/)

### Use

```go
package main

import (
	"fmt"
	"github.com/yisar/cssnext/parser"
)

func main() {
	parser := parser.NewParser()

	s := []byte(".a{color:#fff;}")

	ast := parser.Parse(s)

	fmt.Printf("ast: %s\n", ast.ToPrettyJSON())
	
}
```
