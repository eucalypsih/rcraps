# rcraps
Golang
[1](https://www.w3schools.com/go/go_loops.php) Go For Loops
```golang
package main
import (
  "fmt"
)

func main() {
  var adj = [2]string{"big", "tasty"}
  var fruits = [3]string{"apple", "orange", "banana"}
  for i:=0; i < len(adj); i++ {
    for j:=0; j < len(fruits); j++ {
      fmt.Println(adj[i],fruits[j])
    }
  }
}
```

TypeScript
[1](https://gist.github.com/mstn/5f75651100556dbe30e405691471afe3) Fixed size array in Typescript
```typescript
type FixedSizeArray<N extends number, T, M extends string = '0'> = {
    readonly [k in M]: any;
} & { length: N } & ReadonlyArray<T>;


let adj: FixedSizeArray<2, string>;
adj = ["big", "tasty"];
let fruits: FixedSizeArray<3, string>;
fruits = ["apple", "orange", "banana"];
let i: number;
let j: number;

for ( i = 0; i < adj.length; i++ ) {
    for ( j = 0; j < fruits.length; j++ ) {
        console.log(adj[i], fruits[j]);
    }
}

```
