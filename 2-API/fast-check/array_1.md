[Home](/) &gt; [fast-check](../fast-check.md) &gt; [array](array_1.md)

## array() function

For arrays of values coming from `arb` having an upper bound size

<b>Signature:</b>

```typescript
declare function array<T>(arb: Arbitrary<T>, maxLength: number): Arbitrary<T[]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;T&gt;</code> |  |
|  maxLength | <code>number</code> |  |

<b>Returns:</b>

`Arbitrary<T[]>`

