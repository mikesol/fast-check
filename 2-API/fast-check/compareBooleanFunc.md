[Home](/) &gt; [fast-check](../fast-check.md) &gt; [compareBooleanFunc](compareBooleanFunc.md)

## compareBooleanFunc() function

For comparison boolean functions

A comparison boolean function returns: - true whenever a &lt; b - false otherwise (ie. a = b or a &gt; b)

<b>Signature:</b>

```typescript
export declare function compareBooleanFunc<T>(): Arbitrary<(a: T, b: T) => boolean>;
```
<b>Returns:</b>

`Arbitrary<(a: T, b: T) => boolean>`

