# Interface: HumanReadable

[api/entities/AuthorizationRequest](../wiki/api.entities.AuthorizationRequest).HumanReadable

## Table of contents

### Properties

- [data](../wiki/api.entities.AuthorizationRequest.HumanReadable#data)
- [expiry](../wiki/api.entities.AuthorizationRequest.HumanReadable#expiry)
- [id](../wiki/api.entities.AuthorizationRequest.HumanReadable#id)
- [issuer](../wiki/api.entities.AuthorizationRequest.HumanReadable#issuer)
- [target](../wiki/api.entities.AuthorizationRequest.HumanReadable#target)

## Properties

### data

• **data**: { `type`: [`RotatePrimaryKey`](../wiki/types.AuthorizationType#rotateprimarykey)  } \| { `type`: [`JoinIdentity`](../wiki/types.AuthorizationType#joinidentity) ; `value`: { assets: { values: string[]; type: PermissionType; } \| null; transactions: { exceptions?: TxTag[] \| undefined; values: (TxTag \| ModuleName)[]; type: PermissionType; } \| null; transactionGroups: TxGroup[]; portfolios: { ...; } \| null; }  } \| { `type`: [`PortfolioCustody`](../wiki/types.AuthorizationType#portfoliocustody) ; `value`: { did: string; id?: string \| undefined; }  } \| { `type`: [`BecomeAgent`](../wiki/types.AuthorizationType#becomeagent) ; `value`: { id: string; ticker: string; } \| { type: PermissionGroupType; ticker: string; }  } \| { `type`: [`AddRelayerPayingKey`](../wiki/types.AuthorizationType#addrelayerpayingkey) ; `value`: { beneficiary: string; subsidizer: string; allowance: string; }  } \| { `type`: [`RotatePrimaryKeyToSecondary`](../wiki/types.AuthorizationType#rotateprimarykeytosecondary) ; `value`: { assets: { values: string[]; type: PermissionType; } \| null; transactions: { exceptions?: TxTag[] \| undefined; values: (TxTag \| ModuleName)[]; type: PermissionType; } \| null; transactionGroups: TxGroup[]; portfolios: { ...; } \| null; }  } \| { `type`: [`AttestPrimaryKeyRotation`](../wiki/types.AuthorizationType#attestprimarykeyrotation) \| [`TransferTicker`](../wiki/types.AuthorizationType#transferticker) \| [`AddMultiSigSigner`](../wiki/types.AuthorizationType#addmultisigsigner) \| [`TransferAssetOwnership`](../wiki/types.AuthorizationType#transferassetownership) ; `value`: `string`  }

#### Defined in

[api/entities/AuthorizationRequest.ts:35](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/AuthorizationRequest.ts#L35)

___

### expiry

• **expiry**: ``null`` \| `string`

#### Defined in

[api/entities/AuthorizationRequest.ts:33](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/AuthorizationRequest.ts#L33)

___

### id

• **id**: `string`

#### Defined in

[api/entities/AuthorizationRequest.ts:36](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/AuthorizationRequest.ts#L36)

___

### issuer

• **issuer**: `string`

#### Defined in

[api/entities/AuthorizationRequest.ts:32](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/AuthorizationRequest.ts#L32)

___

### target

• **target**: [`SignerValue`](../wiki/types.SignerValue)

#### Defined in

[api/entities/AuthorizationRequest.ts:34](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/AuthorizationRequest.ts#L34)
