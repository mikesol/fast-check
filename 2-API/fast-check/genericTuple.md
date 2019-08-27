[Home](/) &gt; [fast-check](../fast-check.md) &gt; [genericTuple](genericTuple.md)

## genericTuple() function

For tuples produced by the provided `arbs`

<b>Signature:</b>

```typescript
declare function genericTuple<Ts>(arbs: Arbitrary<Ts>[]): Arbitrary<Ts[]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arbs | <code>Arbitrary&lt;Ts&gt;[]</code> |  |

<b>Returns:</b>

`Arbitrary<Ts[]>`

