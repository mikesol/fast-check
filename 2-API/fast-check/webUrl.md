[Home](/) &gt; [fast-check](../fast-check.md) &gt; [webUrl](webUrl.md)

## webUrl() function

For web url

According to RFC 3986 and WHATWG URL Standard - https://www.ietf.org/rfc/rfc3986.txt - https://url.spec.whatwg.org/

<b>Signature:</b>

```typescript
export declare function webUrl(constraints?: {
    validSchemes?: string[];
    authoritySettings?: WebAuthorityConstraints;
    withQueryParameters?: boolean;
    withFragments?: boolean;
}): import("./definition/Arbitrary").Arbitrary<string>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  constraints | <code>{`<p/>`    validSchemes?: string[];`<p/>`    authoritySettings?: WebAuthorityConstraints;`<p/>`    withQueryParameters?: boolean;`<p/>`    withFragments?: boolean;`<p/>`}</code> |  |

<b>Returns:</b>

`import("./definition/Arbitrary").Arbitrary<string>`

