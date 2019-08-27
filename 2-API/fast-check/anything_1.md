[Home](/) &gt; [fast-check](../fast-check.md) &gt; [anything](anything_1.md)

## anything() function

For any type of values following the constraints defined by `settings`

You may use [sample()](sample.md) to preview the values that will be generated

<b>Signature:</b>

```typescript
declare function anything(settings: ObjectConstraints.Settings): Arbitrary<any>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  settings | <code>ObjectConstraints.Settings</code> |  |

<b>Returns:</b>

`Arbitrary<any>`

#### Example 1

\`\`\`<!-- -->null, undefined, 42, 6.5, 'Hello', {<!-- -->} or {<!-- -->k: \[{<!-- -->}<!-- -->, 1, 2\]<!-- -->}<!-- -->\`\`\`

#### Example 2


```typescript
// Using custom settings
fc.anything({
    key: fc.char(),
    values: [fc.integer(10,20), fc.constant(42)],
    maxDepth: 2
});
// Can build entries such as:
// - 19
// - [{"2":12,"k":15,"A":42}]
// - {"4":[19,13,14,14,42,11,20,11],"6":42,"7":16,"L":10,"'":[20,11],"e":[42,20,42,14,13,17]}
// - [42,42,42]...

```

