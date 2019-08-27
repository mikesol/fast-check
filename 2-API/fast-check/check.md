[Home](/) &gt; [fast-check](../fast-check.md) &gt; [check](check.md)

## check() function

Run the property, do not throw contrary to 

WARNING: Has to be awaited

<b>Signature:</b>

```typescript
declare function check<Ts>(property: AsyncProperty<Ts>, params?: Parameters<Ts>): Promise<RunDetails<Ts>>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  property | <code>AsyncProperty&lt;Ts&gt;</code> |  |
|  params | <code>Parameters&lt;Ts&gt;</code> |  |

<b>Returns:</b>

`Promise<RunDetails<Ts>>`

Test status and other useful details

