[Home](/) &gt; [fast-check](../fast-check.md) &gt; [assert](assert.md)

## assert() function

Run the property, throw in case of failure

It can be called directly from describe/it blocks of Mocha. It does not return anything in case of success.

WARNING: Has to be awaited

<b>Signature:</b>

```typescript
declare function assert<Ts>(property: AsyncProperty<Ts>, params?: Parameters<Ts>): Promise<void>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  property | <code>AsyncProperty&lt;Ts&gt;</code> |  |
|  params | <code>Parameters&lt;Ts&gt;</code> |  |

<b>Returns:</b>

`Promise<void>`

