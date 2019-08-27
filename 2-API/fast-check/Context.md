[Home](/) &gt; [fast-check](../fast-check.md) &gt; [Context](Context.md)

## Context interface

Execution context attached to one predicate run

<b>Signature:</b>

```typescript
export interface Context 
```

## Methods

|  Method | Description |
|  --- | --- |
|  [log(data)](Context.md#log) | Log execution details during a test. Very helpful when troubleshooting failures |
|  [size()](Context.md#size) | Number of logs already logged into current context |

### log

Log execution details during a test. Very helpful when troubleshooting failures

<b>Signature:</b>

```typescript
log(data: string): void;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  data | <code>string</code> |  |

<b>Returns:</b>

`void`

### size

Number of logs already logged into current context

<b>Signature:</b>

```typescript
size(): number;
```
<b>Returns:</b>

`number`

