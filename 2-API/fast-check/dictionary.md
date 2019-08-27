[Home](/) &gt; [fast-check](../fast-check.md) &gt; [dictionary](dictionary.md)

## dictionary() function

For dictionaries with keys produced by `keyArb` and values from `valueArb`

<b>Signature:</b>

```typescript
declare function dictionary<T>(keyArb: Arbitrary<string>, valueArb: Arbitrary<T>): Arbitrary<{
    [key: string]: T;
}>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  keyArb | <code>Arbitrary&lt;string&gt;</code> |  |
|  valueArb | <code>Arbitrary&lt;T&gt;</code> |  |

<b>Returns:</b>

`Arbitrary<{
    [key: string]: T;
}>`

