# Interface: RevokeClaimsParams

[api/procedures/types](../wiki/api.procedures.types).RevokeClaimsParams

## Table of contents

### Properties

- [claims](../wiki/api.procedures.types.RevokeClaimsParams#claims)
- [operation](../wiki/api.procedures.types.RevokeClaimsParams#operation)

## Properties

### claims

• **claims**: `Omit`<[`ClaimTarget`](../wiki/types.ClaimTarget), ``"expiry"``\>[]

array of claims to be revoked

#### Defined in

[api/procedures/types.ts:227](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/procedures/types.ts#L227)

___

### operation

• **operation**: [`Revoke`](../wiki/api.procedures.types.ClaimOperation#revoke)

#### Defined in

[api/procedures/types.ts:228](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/procedures/types.ts#L228)
