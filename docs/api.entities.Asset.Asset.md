# Class: Asset

[api/entities/Asset](../wiki/api.entities.Asset).Asset

Class used to manage all Asset functionality

## Hierarchy

- [`Entity`](../wiki/api.entities.Entity.Entity)<[`UniqueIdentifiers`](../wiki/api.entities.Asset.UniqueIdentifiers), `string`\>

  ↳ **`Asset`**

## Table of contents

### Properties

- [assetHolders](../wiki/api.entities.Asset.Asset#assetholders)
- [checkpoints](../wiki/api.entities.Asset.Asset#checkpoints)
- [compliance](../wiki/api.entities.Asset.Asset#compliance)
- [corporateActions](../wiki/api.entities.Asset.Asset#corporateactions)
- [did](../wiki/api.entities.Asset.Asset#did)
- [documents](../wiki/api.entities.Asset.Asset#documents)
- [issuance](../wiki/api.entities.Asset.Asset#issuance)
- [offerings](../wiki/api.entities.Asset.Asset#offerings)
- [permissions](../wiki/api.entities.Asset.Asset#permissions)
- [settlements](../wiki/api.entities.Asset.Asset#settlements)
- [ticker](../wiki/api.entities.Asset.Asset#ticker)
- [transferRestrictions](../wiki/api.entities.Asset.Asset#transferrestrictions)
- [uuid](../wiki/api.entities.Asset.Asset#uuid)

### Methods

- [controllerTransfer](../wiki/api.entities.Asset.Asset#controllertransfer)
- [createdAt](../wiki/api.entities.Asset.Asset#createdat)
- [currentFundingRound](../wiki/api.entities.Asset.Asset#currentfundinground)
- [details](../wiki/api.entities.Asset.Asset#details)
- [exists](../wiki/api.entities.Asset.Asset#exists)
- [freeze](../wiki/api.entities.Asset.Asset#freeze)
- [getIdentifiers](../wiki/api.entities.Asset.Asset#getidentifiers)
- [getOperationHistory](../wiki/api.entities.Asset.Asset#getoperationhistory)
- [investorCount](../wiki/api.entities.Asset.Asset#investorcount)
- [isEqual](../wiki/api.entities.Asset.Asset#isequal)
- [isFrozen](../wiki/api.entities.Asset.Asset#isfrozen)
- [modify](../wiki/api.entities.Asset.Asset#modify)
- [modifyPrimaryIssuanceAgent](../wiki/api.entities.Asset.Asset#modifyprimaryissuanceagent)
- [redeem](../wiki/api.entities.Asset.Asset#redeem)
- [removePrimaryIssuanceAgent](../wiki/api.entities.Asset.Asset#removeprimaryissuanceagent)
- [toHuman](../wiki/api.entities.Asset.Asset#tohuman)
- [transferOwnership](../wiki/api.entities.Asset.Asset#transferownership)
- [unfreeze](../wiki/api.entities.Asset.Asset#unfreeze)
- [generateUuid](../wiki/api.entities.Asset.Asset#generateuuid)
- [unserialize](../wiki/api.entities.Asset.Asset#unserialize)

## Properties

### assetHolders

• **assetHolders**: [`AssetHolders`](../wiki/api.entities.Asset.AssetHolders.AssetHolders)

#### Defined in

[api/entities/Asset/index.ts:110](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L110)

___

### checkpoints

• **checkpoints**: [`Checkpoints`](../wiki/api.entities.Asset.Checkpoints.Checkpoints)

#### Defined in

[api/entities/Asset/index.ts:115](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L115)

___

### compliance

• **compliance**: [`Compliance`](../wiki/api.entities.Asset.Compliance.Compliance)

#### Defined in

[api/entities/Asset/index.ts:112](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L112)

___

### corporateActions

• **corporateActions**: [`CorporateActions`](../wiki/api.entities.Asset.CorporateActions.CorporateActions)

#### Defined in

[api/entities/Asset/index.ts:116](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L116)

___

### did

• **did**: `string`

Identity ID of the Asset (used for Claims)

#### Defined in

[api/entities/Asset/index.ts:100](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L100)

___

### documents

• **documents**: [`Documents`](../wiki/api.entities.Asset.Documents.Documents)

#### Defined in

[api/entities/Asset/index.ts:108](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L108)

___

### issuance

• **issuance**: [`Issuance`](../wiki/api.entities.Asset.Issuance.Issuance)

#### Defined in

[api/entities/Asset/index.ts:111](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L111)

___

### offerings

• **offerings**: [`Offerings`](../wiki/api.entities.Asset.Offerings.Offerings)

#### Defined in

[api/entities/Asset/index.ts:114](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L114)

___

### permissions

• **permissions**: [`Permissions`](../wiki/api.entities.Asset.Permissions.Permissions)

#### Defined in

[api/entities/Asset/index.ts:117](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L117)

___

### settlements

• **settlements**: [`Settlements`](../wiki/api.entities.Asset.Settlements.Settlements)

#### Defined in

[api/entities/Asset/index.ts:109](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L109)

___

### ticker

• **ticker**: `string`

ticker of the Asset

#### Defined in

[api/entities/Asset/index.ts:105](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L105)

___

### transferRestrictions

• **transferRestrictions**: [`TransferRestrictions`](../wiki/api.entities.Asset.TransferRestrictions.TransferRestrictions)

#### Defined in

[api/entities/Asset/index.ts:113](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Asset/index.ts#L113)

___

### uuid

• **uuid**: `string`

#### Inherited from

[Entity](../wiki/api.entities.Entity.Entity).[uuid](../wiki/api.entities.Entity.Entity#uuid)

#### Defined in

[api/entities/Entity.ts:46](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Entity.ts#L46)

## Methods

### controllerTransfer

▸ **controllerTransfer**(`args`, `opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Force a transfer from a given Portfolio to the caller’s default Portfolio

**`Note`**

 this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [controllerTransfer.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`ControllerTransferParams`](../wiki/api.procedures.types.ControllerTransferParams) |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

___

### createdAt

▸ **createdAt**(): `Promise`<``null`` \| [`EventIdentifier`](../wiki/types.EventIdentifier)\>

Retrieve the identifier data (block number, date and event index) of the event that was emitted when the token was created

**`Note`**

 uses the middleware

**`Note`**

 there is a possibility that the data is not ready by the time it is requested. In that case, `null` is returned

#### Returns

`Promise`<``null`` \| [`EventIdentifier`](../wiki/types.EventIdentifier)\>

___

### currentFundingRound

▸ **currentFundingRound**(): `Promise`<``null`` \| `string`\>

Retrieve the Asset's funding round

**`Note`**

 can be subscribed to

#### Returns

`Promise`<``null`` \| `string`\>

▸ **currentFundingRound**(`callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<``null`` \| `string`\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### details

▸ **details**(): `Promise`<[`AssetDetails`](../wiki/api.entities.Asset.types.AssetDetails)\>

Retrieve the Asset's data

**`Note`**

 can be subscribed to

#### Returns

`Promise`<[`AssetDetails`](../wiki/api.entities.Asset.types.AssetDetails)\>

▸ **details**(`callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<[`AssetDetails`](../wiki/api.entities.Asset.types.AssetDetails)\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### exists

▸ **exists**(): `Promise`<`boolean`\>

Determine whether this Asset exists on chain

#### Returns

`Promise`<`boolean`\>

#### Overrides

[Entity](../wiki/api.entities.Entity.Entity).[exists](../wiki/api.entities.Entity.Entity#exists)

___

### freeze

▸ **freeze**(`opts?`): `Promise`<`TransactionQueue`<[`Asset`](../wiki/api.entities.Asset.Asset), [`Asset`](../wiki/api.entities.Asset.Asset), `unknown`[][]\>\>

Freeze transfers of the Asset

**`Note`**

 this method is of type [NoArgsProcedureMethod](../wiki/types.NoArgsProcedureMethod), which means you can call [freeze.checkAuthorization](../wiki/types.NoArgsProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<[`Asset`](../wiki/api.entities.Asset.Asset), [`Asset`](../wiki/api.entities.Asset.Asset), `unknown`[][]\>\>

___

### getIdentifiers

▸ **getIdentifiers**(): `Promise`<[`SecurityIdentifier`](../wiki/types.SecurityIdentifier)[]\>

Retrieve the Asset's identifiers list

**`Note`**

 can be subscribed to

#### Returns

`Promise`<[`SecurityIdentifier`](../wiki/types.SecurityIdentifier)[]\>

▸ **getIdentifiers**(`callback?`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback?` | [`SubCallback`](../wiki/types#subcallback)<[`SecurityIdentifier`](../wiki/types.SecurityIdentifier)[]\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### getOperationHistory

▸ **getOperationHistory**(): `Promise`<[`HistoricAgentOperation`](../wiki/types.HistoricAgentOperation)[]\>

Retrieve this Asset's Operation History

**`Note`**

 Operations are grouped by the agent Identity who performed them

**`Note`**

 uses the middleware

#### Returns

`Promise`<[`HistoricAgentOperation`](../wiki/types.HistoricAgentOperation)[]\>

___

### investorCount

▸ **investorCount**(): `Promise`<`BigNumber`\>

Retrieve the amount of unique investors that hold this Asset

**`Note`**

 this takes into account the Scope ID of Investor Uniqueness Claims. If an investor holds balances
  of this Asset in two or more different Identities, but they all have Investor Uniqueness Claims with the same
  Scope ID, then they will only be counted once for the purposes of this result

#### Returns

`Promise`<`BigNumber`\>

___

### isEqual

▸ **isEqual**(`entity`): `boolean`

Determine whether this Entity is the same as another one

#### Parameters

| Name | Type |
| :------ | :------ |
| `entity` | [`Entity`](../wiki/api.entities.Entity.Entity)<`unknown`, `unknown`\> |

#### Returns

`boolean`

#### Inherited from

[Entity](../wiki/api.entities.Entity.Entity).[isEqual](../wiki/api.entities.Entity.Entity#isequal)

___

### isFrozen

▸ **isFrozen**(): `Promise`<`boolean`\>

Check whether transfers are frozen for the Asset

**`Note`**

 can be subscribed to

#### Returns

`Promise`<`boolean`\>

▸ **isFrozen**(`callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<`boolean`\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### modify

▸ **modify**(`args`, `opts?`): `Promise`<`TransactionQueue`<[`Asset`](../wiki/api.entities.Asset.Asset), [`Asset`](../wiki/api.entities.Asset.Asset), `unknown`[][]\>\>

Modify some properties of the Asset

**`Throws`**

 if the passed values result in no changes being made to the Asset

**`Note`**

 this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [modify.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`ModifyAssetParams`](../wiki/api.procedures.types#modifyassetparams) |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<[`Asset`](../wiki/api.entities.Asset.Asset), [`Asset`](../wiki/api.entities.Asset.Asset), `unknown`[][]\>\>

___

### modifyPrimaryIssuanceAgent

▸ **modifyPrimaryIssuanceAgent**(`args`, `opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Assign a new primary issuance agent for the Asset

**`Note`**

 this will create an [Authorization Request](../wiki/api.entities.AuthorizationRequest.AuthorizationRequest) which has to be accepted by the `target` Identity.
  An [Account](../wiki/api.entities.Account.Account) or [Identity](../wiki/api.entities.Identity.Identity) can fetch its pending Authorization Requests by calling [authorizations.getReceived](../wiki/api.entities.common.namespaces.Authorizations.Authorizations#getreceived).
  Also, an Account or Identity can directly fetch the details of an Authorization Request by calling [authorizations.getOne](../wiki/api.entities.common.namespaces.Authorizations.Authorizations#getone)

**`Deprecated`**

 in favor of `inviteAgent`

**`Note`**

 this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [modifyPrimaryIssuanceAgent.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`ModifyPrimaryIssuanceAgentParams`](../wiki/api.procedures.types.ModifyPrimaryIssuanceAgentParams) |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

___

### redeem

▸ **redeem**(`args`, `opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Redeem (burn) an amount of this Asset's tokens

**`Note`**

 tokens are removed from the caller's Default Portfolio

**`Note`**

 this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [redeem.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`RedeemTokensParams`](../wiki/api.procedures.types.RedeemTokensParams) |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

___

### removePrimaryIssuanceAgent

▸ **removePrimaryIssuanceAgent**(`opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Remove the primary issuance agent of the Asset

**`Note`**

 if primary issuance agent is not set, Asset owner would be used by default

**`Deprecated`**

 

**`Note`**

 this method is of type [NoArgsProcedureMethod](../wiki/types.NoArgsProcedureMethod), which means you can call [removePrimaryIssuanceAgent.checkAuthorization](../wiki/types.NoArgsProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

___

### toHuman

▸ **toHuman**(): `string`

Return the Asset's ticker

#### Returns

`string`

#### Overrides

[Entity](../wiki/api.entities.Entity.Entity).[toHuman](../wiki/api.entities.Entity.Entity#tohuman)

___

### transferOwnership

▸ **transferOwnership**(`args`, `opts?`): `Promise`<`TransactionQueue`<[`AuthorizationRequest`](../wiki/api.entities.AuthorizationRequest.AuthorizationRequest), [`AuthorizationRequest`](../wiki/api.entities.AuthorizationRequest.AuthorizationRequest), `unknown`[][]\>\>

Transfer ownership of the Asset to another Identity. This generates an authorization request that must be accepted
  by the recipient

**`Note`**

 this will create [Authorization Request](../wiki/api.entities.AuthorizationRequest.AuthorizationRequest) which has to be accepted by the `target` Identity.
  An [Account](../wiki/api.entities.Account.Account) or [Identity](../wiki/api.entities.Identity.Identity) can fetch its pending Authorization Requests by calling [authorizations.getReceived](../wiki/api.entities.common.namespaces.Authorizations.Authorizations#getreceived).
  Also, an Account or Identity can directly fetch the details of an Authorization Request by calling [authorizations.getOne](../wiki/api.entities.common.namespaces.Authorizations.Authorizations#getone)

**`Note`**

 this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [transferOwnership.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | [`TransferAssetOwnershipParams`](../wiki/api.procedures.types.TransferAssetOwnershipParams) |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<[`AuthorizationRequest`](../wiki/api.entities.AuthorizationRequest.AuthorizationRequest), [`AuthorizationRequest`](../wiki/api.entities.AuthorizationRequest.AuthorizationRequest), `unknown`[][]\>\>

___

### unfreeze

▸ **unfreeze**(`opts?`): `Promise`<`TransactionQueue`<[`Asset`](../wiki/api.entities.Asset.Asset), [`Asset`](../wiki/api.entities.Asset.Asset), `unknown`[][]\>\>

Unfreeze transfers of the Asset

**`Note`**

 this method is of type [NoArgsProcedureMethod](../wiki/types.NoArgsProcedureMethod), which means you can call [unfreeze.checkAuthorization](../wiki/types.NoArgsProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<[`Asset`](../wiki/api.entities.Asset.Asset), [`Asset`](../wiki/api.entities.Asset.Asset), `unknown`[][]\>\>

___

### generateUuid

▸ `Static` **generateUuid**<`Identifiers`\>(`identifiers`): `string`

Generate the Entity's UUID from its identifying properties

#### Type parameters

| Name |
| :------ |
| `Identifiers` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `identifiers` | `Identifiers` |

#### Returns

`string`

#### Inherited from

[Entity](../wiki/api.entities.Entity.Entity).[generateUuid](../wiki/api.entities.Entity.Entity#generateuuid)

___

### unserialize

▸ `Static` **unserialize**<`Identifiers`\>(`serialized`): `Identifiers`

Unserialize a UUID into its Unique Identifiers

#### Type parameters

| Name |
| :------ |
| `Identifiers` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serialized` | `string` | UUID to unserialize |

#### Returns

`Identifiers`

#### Inherited from

[Entity](../wiki/api.entities.Entity.Entity).[unserialize](../wiki/api.entities.Entity.Entity#unserialize)
