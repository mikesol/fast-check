[Home](/) &gt; [fast-check](../fast-check.md) &gt; [set](set_4.md)

## set() function

For arrays of unique values coming from `arb` having an upper bound size - unicity defined by `compare`

<b>Signature:</b>

```typescript
declare function set<T>(arb: Arbitrary<T>, maxLength: number, compare: (a: T, b: T) => boolean): Arbitrary<T[]>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  arb | <code>Arbitrary&lt;T&gt;</code> |  |
|  maxLength | <code>number</code> |  |
|  compare | <code>(a: T, b: T) =&gt; boolean</code> |  |

<b>Returns:</b>

`Arbitrary<T[]>`

