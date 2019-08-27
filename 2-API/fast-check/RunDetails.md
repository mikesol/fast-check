[Home](/) &gt; [fast-check](../fast-check.md) &gt; [RunDetails](RunDetails.md)

## RunDetails interface

Post-run details produced by 

A failing property can easily detected by checking the `failed` flag of this structure

<b>Signature:</b>

```typescript
export interface RunDetails<Ts> 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [counterexample](RunDetails.md#counterexample) | <code>Ts &#124; null</code> | In case of failure: the counterexample contains the minimal failing case (first failure after shrinking) |
|  [counterexamplePath](RunDetails.md#counterexamplepath) | <code>string &#124; null</code> | In case of failure: path to the counterexample<!-- -->For replay purposes, it can be forced in , , [sample()](sample.md) and [statistics()](statistics.md) using [Parameters](Parameters.md) |
|  [error](RunDetails.md#error) | <code>string &#124; null</code> | In case of failure: it contains the reason of the failure |
|  [executionSummary](RunDetails.md#executionsummary) | <code>ExecutionTree&lt;Ts&gt;[]</code> | Execution summary of the run<!-- -->Traces the origin of each value encountered during the test and its execution status. Can help to diagnose shrinking issues.<!-- -->You must enable verbose with at least  in [Parameters](Parameters.md) in order to have values in it: - Verbose: Only failures - VeryVerbose: Failures, Successes and Skipped |
|  [failed](RunDetails.md#failed) | <code>boolean</code> | Does the property failed during the execution of ? |
|  [failures](RunDetails.md#failures) | <code>Ts[]</code> | List all failures that have occurred during the run<!-- -->You must enable verbose with at least  in [Parameters](Parameters.md) in order to have values in it |
|  [numRuns](RunDetails.md#numruns) | <code>number</code> | Number of runs<!-- -->- In case of failed property: Number of runs up to the first failure (including the failure run) - Otherwise: Number of successful executions |
|  [numShrinks](RunDetails.md#numshrinks) | <code>number</code> | Number of shrinks required to get to the minimal failing case (aka counterexample) |
|  [numSkips](RunDetails.md#numskips) | <code>number</code> | Number of skipped entries due to failed pre-condition<!-- -->As <code>numRuns</code> it only takes into account the skipped values that occured before the first failure. Refer to [pre](pre.md) to add such pre-conditions. |
|  [seed](RunDetails.md#seed) | <code>number</code> | Seed that have been used by the run<!-- -->It can be forced in , , [sample()](sample.md) and [statistics()](statistics.md) using [Parameters](Parameters.md) |
|  [verbose](RunDetails.md#verbose) | <code>VerbosityLevel</code> | Verbosity level required by the user |

### counterexample

In case of failure: the counterexample contains the minimal failing case (first failure after shrinking)

<b>Signature:</b>

```typescript
counterexample: Ts | null;
```

### counterexamplePath

In case of failure: path to the counterexample

For replay purposes, it can be forced in , , [sample()](sample.md) and [statistics()](statistics.md) using [Parameters](Parameters.md)

<b>Signature:</b>

```typescript
counterexamplePath: string | null;
```

### error

In case of failure: it contains the reason of the failure

<b>Signature:</b>

```typescript
error: string | null;
```

### executionSummary

Execution summary of the run

Traces the origin of each value encountered during the test and its execution status. Can help to diagnose shrinking issues.

You must enable verbose with at least  in [Parameters](Parameters.md) in order to have values in it: - Verbose: Only failures - VeryVerbose: Failures, Successes and Skipped

<b>Signature:</b>

```typescript
executionSummary: ExecutionTree<Ts>[];
```

### failed

Does the property failed during the execution of ?

<b>Signature:</b>

```typescript
failed: boolean;
```

### failures

List all failures that have occurred during the run

You must enable verbose with at least  in [Parameters](Parameters.md) in order to have values in it

<b>Signature:</b>

```typescript
failures: Ts[];
```

### numRuns

Number of runs

- In case of failed property: Number of runs up to the first failure (including the failure run) - Otherwise: Number of successful executions

<b>Signature:</b>

```typescript
numRuns: number;
```

### numShrinks

Number of shrinks required to get to the minimal failing case (aka counterexample)

<b>Signature:</b>

```typescript
numShrinks: number;
```

### numSkips

Number of skipped entries due to failed pre-condition

As `numRuns` it only takes into account the skipped values that occured before the first failure. Refer to [pre](pre.md) to add such pre-conditions.

<b>Signature:</b>

```typescript
numSkips: number;
```

### seed

Seed that have been used by the run

It can be forced in , , [sample()](sample.md) and [statistics()](statistics.md) using [Parameters](Parameters.md)

<b>Signature:</b>

```typescript
seed: number;
```

### verbose

Verbosity level required by the user

<b>Signature:</b>

```typescript
verbose: VerbosityLevel;
```
