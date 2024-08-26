# rcraps
```typescript
type FixedSizeArray<N extends number, T, M extends string = '0'> = {
    readonly [k in M]: any;
} & { length: N } & ReadonlyArray<T>;


let adj: FixedSizeArray<2, string>;
adj = ["big", "tasty"];
let fruits: FixedSizeArray<3, string>;
fruits = ["orange", "apple", "banana"];
let i: number;
let j: number;

for ( i = 0; i < adj.length; i++ ) {
    for ( j = 0; j < fruits.length; j++ ) {
        console.log(adj[i], fruits[j]);
    }
}

```
