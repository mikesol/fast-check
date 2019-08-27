[Home](/) &gt; [fast-check](../fast-check.md) &gt; [webAuthority](webAuthority.md)

## webAuthority() function

For web authority

According to RFC 3986 - https://www.ietf.org/rfc/rfc3986.txt - `authority = [ userinfo "@" ] host [ ":" port ]`

<b>Signature:</b>

```typescript
export declare function webAuthority(constraints?: WebAuthorityConstraints): import("./definition/Arbitrary").Arbitrary<string>;
```

#### Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  constraints | <code>WebAuthorityConstraints</code> |  |

<b>Returns:</b>

`import("./definition/Arbitrary").Arbitrary<string>`

