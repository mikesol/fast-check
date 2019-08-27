[Home](/) &gt; [fast-check](../fast-check.md) &gt; [compareFunc](compareFunc.md)

## compareFunc() function

For comparison functions

A comparison function returns: - negative value whenever a &lt; b - positive value whenever a &gt; b - zero whenever a and b are equivalent

Comparison functions are transitive: `a < b and b < c => a < c`

They also satisfy: `a < b <=> b > a` and `a = b <=> b = a`

<b>Signature:</b>

```typescript
export declare function compareFunc<T>(): Arbitrary<(a: T, b: T) => number>;
```
<b>Returns:</b>

`Arbitrary<(a: T, b: T) => number>`

