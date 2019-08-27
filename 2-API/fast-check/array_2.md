[Home](/) &gt; [fast-check](../fast-check.md) &gt; [array](array_2.md)

## array() function

For arrays of values coming from `arb` having lower and upper bound size

<b>Signature:</b>

```typescript
declare function array<T>(arb: Arbitrary<T>, minLength: number, maxLength: number): Arbitrary<T[]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;T&gt;</code> |  |
|  minLength | <code>number</code> |  |
|  maxLength | <code>number</code> |  |

<b>Returns:</b>

`Arbitrary<T[]>`

