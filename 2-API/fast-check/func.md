[Home](/) &gt; [fast-check](../fast-check.md) &gt; [func](func.md)

## func() function

For pure functions

<b>Signature:</b>

```typescript
export declare function func<TArgs extends any[], TOut>(arb: Arbitrary<TOut>): Arbitrary<(...args: TArgs) => TOut>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;TOut&gt;</code> |  |

<b>Returns:</b>

`Arbitrary<(...args: TArgs) => TOut>`

