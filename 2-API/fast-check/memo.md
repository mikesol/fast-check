[Home](/) &gt; [fast-check](../fast-check.md) &gt; [memo](memo.md)

## memo variable

For mutually recursive types

<b>Signature:</b>

```typescript
memo: <T>(builder: (maxDepth: number) => Arbitrary<T>) => Memo<T>
```

#### Example


```typescript
// tree is 1 / 3 of node, 2 / 3 of leaf
const tree: fc.Memo<Tree> = fc.memo(n => fc.oneof(node(n), leaf(), leaf()));
const node: fc.Memo<Tree> = fc.memo(n => {
  if (n <= 1) return fc.record({ left: leaf(), right: leaf() });
  return fc.record({ left: tree(), right: tree() }); // tree() is equivalent to tree(n-1)
});
const leaf = fc.nat;

```

