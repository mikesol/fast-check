[Home](/) &gt; [fast-check](../fast-check.md) &gt; [WebUrlConstraints](WebUrlConstraints.md)

## WebUrlConstraints interface

<b>Signature:</b>

```typescript
export interface WebUrlConstraints 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [authoritySettings](WebUrlConstraints.md#authoritysettings) | <code>WebAuthorityConstraints</code> | Settings for  |
|  [validSchemes](WebUrlConstraints.md#validschemes) | <code>string[]</code> | Enforce specific schemes, eg.: http, https |
|  [withFragments](WebUrlConstraints.md#withfragments) | <code>boolean</code> | Enable fragments in the generated url |
|  [withQueryParameters](WebUrlConstraints.md#withqueryparameters) | <code>boolean</code> | Enable query parameters in the generated url |

### authoritySettings

Settings for 

<b>Signature:</b>

```typescript
authoritySettings?: WebAuthorityConstraints;
```

### validSchemes

Enforce specific schemes, eg.: http, https

<b>Signature:</b>

```typescript
validSchemes?: string[];
```

### withFragments

Enable fragments in the generated url

<b>Signature:</b>

```typescript
withFragments?: boolean;
```

### withQueryParameters

Enable query parameters in the generated url

<b>Signature:</b>

```typescript
withQueryParameters?: boolean;
```
