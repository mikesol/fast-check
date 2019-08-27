[Home](/) &gt; [fast-check](../fast-check.md) &gt; [assert](assert_1.md)

## assert() function

Run the property, throw in case of failure

It can be called directly from describe/it blocks of Mocha. It does not return anything in case of success.

<b>Signature:</b>

```typescript
declare function assert<Ts>(property: Property<Ts>, params?: Parameters<Ts>): void;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  property | <code>Property&lt;Ts&gt;</code> |  |
|  params | <code>Parameters&lt;Ts&gt;</code> |  |

<b>Returns:</b>

`void`

