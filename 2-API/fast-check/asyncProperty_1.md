[Home](/) &gt; [fast-check](../fast-check.md) &gt; [asyncProperty](asyncProperty_1.md)

## asyncProperty() function

Instantiate a new 

<b>Signature:</b>

```typescript
declare function asyncProperty<T0, T1>(arb0: Arbitrary<T0>, arb1: Arbitrary<T1>, predicate: (t0: T0, t1: T1) => Promise<boolean | void>): AsyncProperty<[T0, T1]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb0 | <code>Arbitrary&lt;T0&gt;</code> |  |
|  arb1 | <code>Arbitrary&lt;T1&gt;</code> |  |
|  predicate | <code>(t0: T0, t1: T1) =&gt; Promise&lt;boolean &#124; void&gt;</code> |  |

<b>Returns:</b>

`AsyncProperty<[T0, T1]>`

