[Home](/) &gt; [fast-check](../fast-check.md) &gt; [set](set_1.md)

## set() function

For arrays of unique values coming from `arb` having an upper bound size

<b>Signature:</b>

```typescript
declare function set<T>(arb: Arbitrary<T>, maxLength: number): Arbitrary<T[]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;T&gt;</code> |  |
|  maxLength | <code>number</code> |  |

<b>Returns:</b>

`Arbitrary<T[]>`

