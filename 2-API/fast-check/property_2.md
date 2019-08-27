[Home](/) &gt; [fast-check](../fast-check.md) &gt; [property](property_2.md)

## property() function

Instantiate a new 

<b>Signature:</b>

```typescript
declare function property<T0, T1, T2>(arb0: Arbitrary<T0>, arb1: Arbitrary<T1>, arb2: Arbitrary<T2>, predicate: (t0: T0, t1: T1, t2: T2) => (boolean | void)): Property<[T0, T1, T2]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb0 | <code>Arbitrary&lt;T0&gt;</code> |  |
|  arb1 | <code>Arbitrary&lt;T1&gt;</code> |  |
|  arb2 | <code>Arbitrary&lt;T2&gt;</code> |  |
|  predicate | <code>(t0: T0, t1: T1, t2: T2) =&gt; (boolean &#124; void)</code> |  |

<b>Returns:</b>

`Property<[T0, T1, T2]>`

