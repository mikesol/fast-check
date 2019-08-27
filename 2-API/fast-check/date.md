[Home](/) &gt; [fast-check](../fast-check.md) &gt; [date](date.md)

## date() function

For date between constraints.min or new Date(-8640000000000000) (included) and constraints.max or new Date(8640000000000000) (included)

<b>Signature:</b>

```typescript
export declare function date(constraints?: {
    min?: Date;
    max?: Date;
}): Arbitrary<Date>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  constraints | <code>{`<p/>`    min?: Date;`<p/>`    max?: Date;`<p/>`}</code> |  |

<b>Returns:</b>

`Arbitrary<Date>`

