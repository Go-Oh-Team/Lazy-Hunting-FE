# LazyHunting_FE
```c++
if(lazy[node]){
  tree[node] += (end - start + 1) * lazy[node];
  if(start != end){
    lazy[node<<1] += lazy[node];
    lazy[(node<<1)|1] += lazy[node];
  }
lazy[node] = 0;
}
```
