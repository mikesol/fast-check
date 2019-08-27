[Home](/) &gt; [fast-check](../fast-check.md) &gt; [property](property.md)

## property() function

Instantiate a new 

<b>Signature:</b>

```typescript
declare function property<T0>(arb0: Arbitrary<T0>, predicate: (t0: T0) => (boolean | void)): Property<[T0]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb0 | <code>Arbitrary&lt;T0&gt;</code> |  |
|  predicate | <code>(t0: T0) =&gt; (boolean &#124; void)</code> |  |

<b>Returns:</b>

`Property<[T0]>`

