[Home](/) &gt; [fast-check](../fast-check.md) &gt; [object](object_1.md)

## object() function

For any objects following the constraints defined by `settings`

You may use [sample()](sample.md) to preview the values that will be generated

<b>Signature:</b>

```typescript
declare function object(settings: ObjectConstraints.Settings): Arbitrary<any>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  settings | <code>ObjectConstraints.Settings</code> |  |

<b>Returns:</b>

`Arbitrary<any>`

#### Example

\`\`\`<!-- -->{<!-- -->} or {<!-- -->k: \[{<!-- -->}<!-- -->, 1, 2\]<!-- -->}<!-- -->\`\`\`

