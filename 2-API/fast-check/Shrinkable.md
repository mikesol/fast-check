[Home](/) &gt; [fast-check](../fast-check.md) &gt; [Shrinkable](Shrinkable.md)

## Shrinkable class

A Shrinkable<T> holds an internal value of type `T` and can shrink it to smaller `T` values

<b>Signature:</b>

```typescript
export declare class Shrinkable<T> 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [hasToBeCloned](Shrinkable.md#hastobecloned) | <code>boolean</code> | State storing the result of hasCloneMethod If <true> the value will be cloned each time it gets accessed |
|  [shrink](Shrinkable.md#shrink) | <code>() =&gt; Stream&lt;Shrinkable&lt;T&gt;&gt;</code> |  |
|  [value\_](Shrinkable.md#value_) | <code>T</code> |  |
|  [value](Shrinkable.md#value) | <code>T</code> | Safe value of the shrinkable Depending on  it will either be  or a clone of it |

### hasToBeCloned

State storing the result of hasCloneMethod If <true> the value will be cloned each time it gets accessed

<b>Signature:</b>

```typescript
readonly hasToBeCloned: boolean;
```

### shrink

<b>Signature:</b>

```typescript
readonly shrink: () => Stream<Shrinkable<T>>;
```

### value\_

<b>Signature:</b>

```typescript
readonly value_: T;
```

### value

Safe value of the shrinkable Depending on  it will either be  or a clone of it

<b>Signature:</b>

```typescript
readonly value: T;
```

## Methods

|  Method | Description |
|  --- | --- |
|  [filter(predicate)](Shrinkable.md#filter) | Create another shrinkable by filtering its shrunk values against <code>predicate</code>All the shrunk values produced by the resulting <code>Shrinkable&lt;T&gt;</code> satisfy <code>predicate(value) == true</code> |
|  [map(mapper)](Shrinkable.md#map) | Create another shrinkable by mapping all values using the provided <code>mapper</code> Both the original value and the shrunk ones are impacted |

### filter

Create another shrinkable by filtering its shrunk values against `predicate`

All the shrunk values produced by the resulting `Shrinkable<T>` satisfy `predicate(value) == true`

<b>Signature:</b>

```typescript
filter(predicate: (t: T) => boolean): Shrinkable<T>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  predicate | <code>(t: T) =&gt; boolean</code> |  |

<b>Returns:</b>

`Shrinkable<T>`

New shrinkable filtered using predicate

### map

Create another shrinkable by mapping all values using the provided `mapper` Both the original value and the shrunk ones are impacted

<b>Signature:</b>

```typescript
map<U>(mapper: (t: T) => U): Shrinkable<U>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  mapper | <code>(t: T) =&gt; U</code> |  |

<b>Returns:</b>

`Shrinkable<U>`

New shrinkable with mapped elements

