[Home](/) &gt; [fast-check](../fast-check.md) &gt; [record](record.md)

## record() function

For records following the `recordModel` schema

<b>Signature:</b>

```typescript
declare function record<T>(recordModel: {
    [K in keyof T]: Arbitrary<T[K]>;
}): Arbitrary<{
    [K in keyof T]: T[K];
}>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  recordModel | <code>{`<p/>`    [K in keyof T]: Arbitrary&lt;T[K]&gt;;`<p/>`}</code> |  |

<b>Returns:</b>

`Arbitrary<{
    [K in keyof T]: T[K];
}>`

#### Example


```typescript
record({ x: someArbitraryInt, y: someArbitraryInt }): Arbitrary<{x:number,y:number}>
// merge two integer arbitraries to produce a {x, y} record

```

