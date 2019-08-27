[Home](/) &gt; [fast-check](../fast-check.md) &gt; [asyncProperty](asyncProperty.md)

## asyncProperty() function

Instantiate a new 

<b>Signature:</b>

```typescript
declare function asyncProperty<T0>(arb0: Arbitrary<T0>, predicate: (t0: T0) => Promise<boolean | void>): AsyncProperty<[T0]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb0 | <code>Arbitrary&lt;T0&gt;</code> |  |
|  predicate | <code>(t0: T0) =&gt; Promise&lt;boolean &#124; void&gt;</code> |  |

<b>Returns:</b>

`AsyncProperty<[T0]>`

