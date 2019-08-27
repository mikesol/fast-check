[Home](/) &gt; [fast-check](../fast-check.md) &gt; [check](check_1.md)

## check() function

Run the property, do not throw contrary to 

<b>Signature:</b>

```typescript
declare function check<Ts>(property: Property<Ts>, params?: Parameters<Ts>): RunDetails<Ts>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  property | <code>Property&lt;Ts&gt;</code> |  |
|  params | <code>Parameters&lt;Ts&gt;</code> |  |

<b>Returns:</b>

`RunDetails<Ts>`

Test status and other useful details

