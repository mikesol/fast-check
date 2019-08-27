[Home](/) &gt; [fast-check](../../fast-check.md) &gt; [ObjectConstraints](../ObjectConstraints.md) &gt; [Settings](Settings.md)

## ObjectConstraints.Settings interface

Constraints to be applied during object generation

<b>Signature:</b>

```typescript
interface Settings 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [key](Settings.md#key) | <code>Arbitrary&lt;string&gt;</code> | Arbitrary for keys<!-- -->Default for <code>key</code> is: <code>fc.string()</code> |
|  [maxDepth](Settings.md#maxdepth) | <code>number</code> | Maximal depth allowed |
|  [maxKeys](Settings.md#maxkeys) | <code>number</code> | Maximal number of keys |
|  [values](Settings.md#values) | <code>Arbitrary&lt;any&gt;[]</code> | Arbitrary for values<!-- -->Default for <code>values</code> are: - <code>fc.boolean()</code>, - <code>fc.integer()</code>, - <code>fc.double()</code>, - <code>fc.string()</code> - constants among: - <code>null</code>, - <code>undefined</code>, - <code>Number.NaN</code>, - <code>+0</code>, - <code>-0</code>, - <code>Number.EPSILON</code>, - <code>Number.MIN_VALUE</code>, - <code>Number.MAX_VALUE</code>, - <code>Number.MIN_SAFE_INTEGER</code>, - <code>Number.MAX_SAFE_INTEGER</code>, - <code>Number.POSITIVE_INFINITY</code>, - <code>Number.NEGATIVE_INFINITY</code> |
|  [withBoxedValues](Settings.md#withboxedvalues) | <code>boolean</code> | Also generate boxed versions of values |
|  [withMap](Settings.md#withmap) | <code>boolean</code> | Also generate Map |
|  [withSet](Settings.md#withset) | <code>boolean</code> | Also generate Set |

### key

Arbitrary for keys

Default for `key` is: `fc.string()`

<b>Signature:</b>

```typescript
key?: Arbitrary<string>;
```

### maxDepth

Maximal depth allowed

<b>Signature:</b>

```typescript
maxDepth?: number;
```

### maxKeys

Maximal number of keys

<b>Signature:</b>

```typescript
maxKeys?: number;
```

### values

Arbitrary for values

Default for `values` are: - `fc.boolean()`<!-- -->, - `fc.integer()`<!-- -->, - `fc.double()`<!-- -->, - `fc.string()` - constants among: - `null`<!-- -->, - `undefined`<!-- -->, - `Number.NaN`<!-- -->, - `+0`<!-- -->, - `-0`<!-- -->, - `Number.EPSILON`<!-- -->, - `Number.MIN_VALUE`<!-- -->, - `Number.MAX_VALUE`<!-- -->, - `Number.MIN_SAFE_INTEGER`<!-- -->, - `Number.MAX_SAFE_INTEGER`<!-- -->, - `Number.POSITIVE_INFINITY`<!-- -->, - `Number.NEGATIVE_INFINITY`

<b>Signature:</b>

```typescript
values?: Arbitrary<any>[];
```

### withBoxedValues

Also generate boxed versions of values

<b>Signature:</b>

```typescript
withBoxedValues?: boolean;
```

### withMap

Also generate Map

<b>Signature:</b>

```typescript
withMap?: boolean;
```

### withSet

Also generate Set

<b>Signature:</b>

```typescript
withSet?: boolean;
```
