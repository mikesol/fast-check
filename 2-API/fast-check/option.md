[Home](/) &gt; [fast-check](../fast-check.md) &gt; [option](option.md)

## option() function

For either null or a value coming from `arb`

<b>Signature:</b>

```typescript
declare function option<T>(arb: Arbitrary<T>): Arbitrary<T | null>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;T&gt;</code> |  |

<b>Returns:</b>

`Arbitrary<T | null>`

