[Home](/) &gt; [fast-check](../fast-check.md) &gt; [Parameters](Parameters.md)

## Parameters interface

Customization of the parameters used to run the properties

<b>Signature:</b>

```typescript
export interface Parameters<T = void> 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [endOnFailure](Parameters.md#endonfailure) | <code>boolean</code> | Stop run on failure<!-- -->It makes the run stop at the first encountered failure without shrinking.<!-- -->When used in complement to <code>seed</code> and <code>path</code>, it replays only the minimal counterexample. |
|  [examples](Parameters.md#examples) | <code>T[]</code> | Custom values added at the beginning of generated ones<!-- -->It enables users to come with examples they want to test at every run |
|  [maxSkipsPerRun](Parameters.md#maxskipsperrun) | <code>number</code> | Maximal number of skipped values per run<!-- -->Skipped is considered globally, so this value is used to compute maxSkips = maxSkipsPerRun \* numRuns. Runner will consider a run to have failed if it skipped maxSkips+1 times before having generated numRuns valid entries.<!-- -->See [pre](pre.md) for more details on pre-conditions |
|  [numRuns](Parameters.md#numruns) | <code>number</code> | Number of runs before success: 100 by default |
|  [path](Parameters.md#path) | <code>string</code> | Way to replay a failing property directly with the counterexample. It can be fed with the counterexamplePath returned by the failing test (requires <code>seed</code> too). |
|  [randomType](Parameters.md#randomtype) | <code>RandomType &#124; ((seed: number) =&gt; RandomGenerator)</code> | Random number generator: <code>xorshift128plus</code> by default<!-- -->Random generator is the core element behind the generation of random values - changing it might directly impact the quality and performances of the generation of random values. It can be one of: 'mersenne', 'congruential', 'congruential32', 'xorshift128plus' Or any function able to build a <code>RandomGenerator</code> based on a seed |
|  [seed](Parameters.md#seed) | <code>number</code> | Initial seed of the generator: <code>Date.now()</code> by default<!-- -->It can be forced to replay a failed run.<!-- -->In theory, seeds are supposed to be 32 bits integers. In case of double value, the seed will be rescaled into a valid 32 bits integer (eg.: values between 0 and 1 will be evenly spread into the range of possible seeds). |
|  [skipAllAfterTimeLimit](Parameters.md#skipallaftertimelimit) | <code>number</code> | Skip all runs after a given time limit: disabled by default<!-- -->NOTE: Relies on <code>Date.now()</code>.<!-- -->NOTE: Useful to stop too long shrinking processes. Replay capability (see , ) can resume the shrinking.<!-- -->WARNING: It skips runs. Thus test might be marked as failed. Indeed, it might not reached the requested number of successful runs. |
|  [timeout](Parameters.md#timeout) | <code>number</code> | Maximum time in milliseconds for the predicate to answer: disabled by default<!-- -->WARNING: Only works for async code (see ), will not interrupt a synchronous code. |
|  [unbiased](Parameters.md#unbiased) | <code>boolean</code> | Force the use of unbiased arbitraries: biased by default |
|  [verbose](Parameters.md#verbose) | <code>boolean &#124; VerbosityLevel</code> | Enable verbose mode: [VerbosityLevel.None](VerbosityLevel/None.md) by default<!-- -->Using <code>verbose: true</code> is equivalent to <code>verbose: VerbosityLevel.Verbose</code>It can prove very useful to troubleshoot issues. See [VerbosityLevel](VerbosityLevel.md) for more details on each level. |

### endOnFailure

Stop run on failure

It makes the run stop at the first encountered failure without shrinking.

When used in complement to `seed` and `path`<!-- -->, it replays only the minimal counterexample.

<b>Signature:</b>

```typescript
endOnFailure?: boolean;
```

### examples

Custom values added at the beginning of generated ones

It enables users to come with examples they want to test at every run

<b>Signature:</b>

```typescript
examples?: T[];
```

### maxSkipsPerRun

Maximal number of skipped values per run

Skipped is considered globally, so this value is used to compute maxSkips = maxSkipsPerRun \* numRuns. Runner will consider a run to have failed if it skipped maxSkips+1 times before having generated numRuns valid entries.

See [pre](pre.md) for more details on pre-conditions

<b>Signature:</b>

```typescript
maxSkipsPerRun?: number;
```

### numRuns

Number of runs before success: 100 by default

<b>Signature:</b>

```typescript
numRuns?: number;
```

### path

Way to replay a failing property directly with the counterexample. It can be fed with the counterexamplePath returned by the failing test (requires `seed` too).

<b>Signature:</b>

```typescript
path?: string;
```

### randomType

Random number generator: `xorshift128plus` by default

Random generator is the core element behind the generation of random values - changing it might directly impact the quality and performances of the generation of random values. It can be one of: 'mersenne', 'congruential', 'congruential32', 'xorshift128plus' Or any function able to build a `RandomGenerator` based on a seed

<b>Signature:</b>

```typescript
randomType?: RandomType | ((seed: number) => RandomGenerator);
```

### seed

Initial seed of the generator: `Date.now()` by default

It can be forced to replay a failed run.

In theory, seeds are supposed to be 32 bits integers. In case of double value, the seed will be rescaled into a valid 32 bits integer (eg.: values between 0 and 1 will be evenly spread into the range of possible seeds).

<b>Signature:</b>

```typescript
seed?: number;
```

### skipAllAfterTimeLimit

Skip all runs after a given time limit: disabled by default

NOTE: Relies on `Date.now()`<!-- -->.

NOTE: Useful to stop too long shrinking processes. Replay capability (see , ) can resume the shrinking.

WARNING: It skips runs. Thus test might be marked as failed. Indeed, it might not reached the requested number of successful runs.

<b>Signature:</b>

```typescript
skipAllAfterTimeLimit?: number;
```

### timeout

Maximum time in milliseconds for the predicate to answer: disabled by default

WARNING: Only works for async code (see ), will not interrupt a synchronous code.

<b>Signature:</b>

```typescript
timeout?: number;
```

### unbiased

Force the use of unbiased arbitraries: biased by default

<b>Signature:</b>

```typescript
unbiased?: boolean;
```

### verbose

Enable verbose mode: [VerbosityLevel.None](VerbosityLevel/None.md) by default

Using `verbose: true` is equivalent to `verbose: VerbosityLevel.Verbose`

It can prove very useful to troubleshoot issues. See [VerbosityLevel](VerbosityLevel.md) for more details on each level.

<b>Signature:</b>

```typescript
verbose?: boolean | VerbosityLevel;
```

## Methods

|  Method | Description |
|  --- | --- |
|  [logger(v)](Parameters.md#logger) | Logger (see [statistics()](statistics.md)<!-- -->): <code>console.log</code> by default |

### logger

Logger (see [statistics()](statistics.md)<!-- -->): `console.log` by default

<b>Signature:</b>

```typescript
logger?(v: string): void;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  v | <code>string</code> |  |

<b>Returns:</b>

`void`

