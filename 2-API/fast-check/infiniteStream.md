[Home](/) &gt; [fast-check](../fast-check.md) &gt; [infiniteStream](infiniteStream.md)

## infiniteStream() function

Produce an infinite stream of values

WARNING: Requires Object.assign

<b>Signature:</b>

```typescript
declare function infiniteStream<T>(arb: Arbitrary<T>): Arbitrary<Stream<T>>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;T&gt;</code> |  |

<b>Returns:</b>

`Arbitrary<Stream<T>>`

