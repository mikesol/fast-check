[Home](/) &gt; [fast-check](../fast-check.md) &gt; [sample](sample.md)

## sample() function

Generate an array containing all the values that would have been generated during  or 

<b>Signature:</b>

```typescript
declare function sample<Ts>(generator: IProperty<Ts> | Arbitrary<Ts>, params?: Parameters<Ts> | number): Ts[];
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  generator | <code>IProperty&lt;Ts&gt; &#124; Arbitrary&lt;Ts&gt;</code> |  |
|  params | <code>Parameters&lt;Ts&gt; &#124; number</code> |  |

<b>Returns:</b>

`Ts[]`

#### Example


```typescript
fc.sample(fc.nat(), 10); // extract 10 values from fc.nat() Arbitrary
fc.sample(fc.nat(), {seed: 42}); // extract values from fc.nat() as if we were running fc.assert with seed=42

```

