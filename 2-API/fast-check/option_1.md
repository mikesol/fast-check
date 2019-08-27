[Home](/) &gt; [fast-check](../fast-check.md) &gt; [option](option_1.md)

## option() function

For either null or a value coming from `arb` with custom frequency

<b>Signature:</b>

```typescript
declare function option<T>(arb: Arbitrary<T>, freq: number): Arbitrary<T | null>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;T&gt;</code> |  |
|  freq | <code>number</code> |  |

<b>Returns:</b>

`Arbitrary<T | null>`

