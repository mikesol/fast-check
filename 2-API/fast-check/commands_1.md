[Home](/) &gt; [fast-check](../fast-check.md) &gt; [commands](commands_1.md)

## commands() function

For arrays of [Command](Command.md) to be executed by [modelRun](modelRun.md)

This implementation comes with a shrinker adapted for commands. It should shrink more efficiently than  for [Command](Command.md) arrays.

<b>Signature:</b>

```typescript
declare function commands<Model extends object, Real>(commandArbs: Arbitrary<Command<Model, Real>>[], maxCommands?: number): Arbitrary<Iterable<Command<Model, Real>>>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  commandArbs | <code>Arbitrary&lt;Command&lt;Model, Real&gt;&gt;[]</code> |  |
|  maxCommands | <code>number</code> |  |

<b>Returns:</b>

`Arbitrary<Iterable<Command<Model, Real>>>`

