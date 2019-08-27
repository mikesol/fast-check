[Home](/) &gt; [fast-check](../fast-check.md) &gt; [property](property_1.md)

## property() function

Instantiate a new 

<b>Signature:</b>

```typescript
declare function property<T0, T1>(arb0: Arbitrary<T0>, arb1: Arbitrary<T1>, predicate: (t0: T0, t1: T1) => (boolean | void)): Property<[T0, T1]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb0 | <code>Arbitrary&lt;T0&gt;</code> |  |
|  arb1 | <code>Arbitrary&lt;T1&gt;</code> |  |
|  predicate | <code>(t0: T0, t1: T1) =&gt; (boolean &#124; void)</code> |  |

<b>Returns:</b>

`Property<[T0, T1]>`

