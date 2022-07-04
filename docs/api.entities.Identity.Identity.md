# Class: Identity

[api/entities/Identity](../wiki/api.entities.Identity).Identity

Represents an Identity in the Polymesh blockchain

## Hierarchy

- [`Entity`](../wiki/api.entities.Entity.Entity)<[`UniqueIdentifiers`](../wiki/api.entities.Identity.UniqueIdentifiers), `string`\>

  ↳ **`Identity`**

  ↳↳ [`DefaultTrustedClaimIssuer`](../wiki/api.entities.DefaultTrustedClaimIssuer.DefaultTrustedClaimIssuer)

## Table of contents

### Properties

- [assetPermissions](../wiki/api.entities.Identity.Identity#assetpermissions)
- [authorizations](../wiki/api.entities.Identity.Identity#authorizations)
- [did](../wiki/api.entities.Identity.Identity#did)
- [portfolios](../wiki/api.entities.Identity.Identity#portfolios)
- [uuid](../wiki/api.entities.Identity.Identity#uuid)

### Methods

- [areSecondaryAccountsFrozen](../wiki/api.entities.Identity.Identity#aresecondaryaccountsfrozen)
- [checkRoles](../wiki/api.entities.Identity.Identity#checkroles)
- [exists](../wiki/api.entities.Identity.Identity#exists)
- [getAssetBalance](../wiki/api.entities.Identity.Identity#getassetbalance)
- [getHeldAssets](../wiki/api.entities.Identity.Identity#getheldassets)
- [getInstructions](../wiki/api.entities.Identity.Identity#getinstructions)
- [getPendingDistributions](../wiki/api.entities.Identity.Identity#getpendingdistributions)
- [getPendingInstructions](../wiki/api.entities.Identity.Identity#getpendinginstructions)
- [getPrimaryAccount](../wiki/api.entities.Identity.Identity#getprimaryaccount)
- [getScopeId](../wiki/api.entities.Identity.Identity#getscopeid)
- [getSecondaryAccounts](../wiki/api.entities.Identity.Identity#getsecondaryaccounts)
- [getTrustingAssets](../wiki/api.entities.Identity.Identity#gettrustingassets)
- [getVenues](../wiki/api.entities.Identity.Identity#getvenues)
- [hasRole](../wiki/api.entities.Identity.Identity#hasrole)
- [hasRoles](../wiki/api.entities.Identity.Identity#hasroles)
- [hasValidCdd](../wiki/api.entities.Identity.Identity#hasvalidcdd)
- [isCddProvider](../wiki/api.entities.Identity.Identity#iscddprovider)
- [isEqual](../wiki/api.entities.Identity.Identity#isequal)
- [isGcMember](../wiki/api.entities.Identity.Identity#isgcmember)
- [toHuman](../wiki/api.entities.Identity.Identity#tohuman)
- [generateUuid](../wiki/api.entities.Identity.Identity#generateuuid)
- [unserialize](../wiki/api.entities.Identity.Identity#unserialize)

## Properties

### assetPermissions

• **assetPermissions**: [`AssetPermissions`](../wiki/api.entities.Identity.AssetPermissions.AssetPermissions)

#### Defined in

[api/entities/Identity/index.ts:99](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Identity/index.ts#L99)

___

### authorizations

• **authorizations**: [`IdentityAuthorizations`](../wiki/api.entities.Identity.IdentityAuthorizations.IdentityAuthorizations)

#### Defined in

[api/entities/Identity/index.ts:97](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Identity/index.ts#L97)

___

### did

• **did**: `string`

Identity ID as stored in the blockchain

#### Defined in

[api/entities/Identity/index.ts:94](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Identity/index.ts#L94)

___

### portfolios

• **portfolios**: [`Portfolios`](../wiki/api.entities.Identity.Portfolios.Portfolios)

#### Defined in

[api/entities/Identity/index.ts:98](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Identity/index.ts#L98)

___

### uuid

• **uuid**: `string`

#### Inherited from

[Entity](../wiki/api.entities.Entity.Entity).[uuid](../wiki/api.entities.Entity.Entity#uuid)

#### Defined in

[api/entities/Entity.ts:46](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/Entity.ts#L46)

## Methods

### areSecondaryAccountsFrozen

▸ **areSecondaryAccountsFrozen**(): `Promise`<`boolean`\>

Check whether secondary Accounts are frozen

**`Note`**

 can be subscribed to

#### Returns

`Promise`<`boolean`\>

▸ **areSecondaryAccountsFrozen**(`callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<`boolean`\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### checkRoles

▸ **checkRoles**(`roles`): `Promise`<[`CheckRolesResult`](../wiki/types.CheckRolesResult)\>

Check whether this Identity possesses all specified roles

#### Parameters

| Name | Type |
| :------ | :------ |
| `roles` | [`Role`](../wiki/types#role)[] |

#### Returns

`Promise`<[`CheckRolesResult`](../wiki/types.CheckRolesResult)\>

___

### exists

▸ **exists**(): `Promise`<`boolean`\>

Determine whether this Identity exists on chain

**`Note`**

 asset Identities aren't considered to exist for the

#### Returns

`Promise`<`boolean`\>

#### Overrides

[Entity](../wiki/api.entities.Entity.Entity).[exists](../wiki/api.entities.Entity.Entity#exists)

___

### getAssetBalance

▸ **getAssetBalance**(`args`): `Promise`<`BigNumber`\>

Retrieve the balance of a particular Asset

**`Note`**

 can be subscribed to

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Object` |
| `args.ticker` | `string` |

#### Returns

`Promise`<`BigNumber`\>

▸ **getAssetBalance**(`args`, `callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Object` |
| `args.ticker` | `string` |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<`BigNumber`\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### getHeldAssets

▸ **getHeldAssets**(`opts?`): `Promise`<[`ResultSet`](../wiki/types.ResultSet)<[`Asset`](../wiki/api.entities.Asset.Asset)\>\>

Retrieve a list of all Assets which were held at one point by this Identity

**`Note`**

 uses the middleware

**`Note`**

 supports pagination

#### Parameters

| Name | Type |
| :------ | :------ |
| `opts` | `Object` |
| `opts.order?` | [`Order`](../wiki/types.Order) |
| `opts.size?` | `BigNumber` |
| `opts.start?` | `BigNumber` |

#### Returns

`Promise`<[`ResultSet`](../wiki/types.ResultSet)<[`Asset`](../wiki/api.entities.Asset.Asset)\>\>

___

### getInstructions

▸ **getInstructions**(): `Promise`<[`GroupedInstructions`](../wiki/types.GroupedInstructions)\>

Retrieve all Instructions where this Identity is a participant,
  grouped by status

#### Returns

`Promise`<[`GroupedInstructions`](../wiki/types.GroupedInstructions)\>

___

### getPendingDistributions

▸ **getPendingDistributions**(): `Promise`<[`DistributionWithDetails`](../wiki/types.DistributionWithDetails)[]\>

Retrieve every Dividend Distribution for which this Identity is eligible and hasn't been paid

**`Note`**

 uses the middleware

**`Note`**

 this query can be potentially **SLOW** depending on which Assets this Identity has held

#### Returns

`Promise`<[`DistributionWithDetails`](../wiki/types.DistributionWithDetails)[]\>

___

### getPendingInstructions

▸ **getPendingInstructions**(): `Promise`<[`Instruction`](../wiki/api.entities.Instruction.Instruction)[]\>

Retrieve all pending Instructions involving this Identity

**`Deprecated`**

 in favor of `getInstructions`

#### Returns

`Promise`<[`Instruction`](../wiki/api.entities.Instruction.Instruction)[]\>

___

### getPrimaryAccount

▸ **getPrimaryAccount**(): `Promise`<[`PermissionedAccount`](../wiki/types.PermissionedAccount)\>

Retrieve the primary Account associated with the Identity

**`Note`**

 can be subscribed to

#### Returns

`Promise`<[`PermissionedAccount`](../wiki/types.PermissionedAccount)\>

▸ **getPrimaryAccount**(`callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<[`PermissionedAccount`](../wiki/types.PermissionedAccount)\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### getScopeId

▸ **getScopeId**(`args`): `Promise`<``null`` \| `string`\>

Retrieve the Scope ID associated to this Identity's Investor Uniqueness Claim for a specific Asset, or null
  if there is none

**`Note`**

 more on Investor Uniqueness [here](https://developers.polymesh.network/introduction/identity#polymesh-unique-identity-system-puis) and
  [here](https://developers.polymesh.network/polymesh-docs/primitives/confidential-identity)

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Object` |
| `args.asset` | `string` \| [`Asset`](../wiki/api.entities.Asset.Asset) |

#### Returns

`Promise`<``null`` \| `string`\>

___

### getSecondaryAccounts

▸ **getSecondaryAccounts**(): `Promise`<[`PermissionedAccount`](../wiki/types.PermissionedAccount)[]\>

Get the list of secondary Accounts related to the Identity

**`Note`**

 can be subscribed to

**`Note`**

 This method currently lacks pagination and may be slow for identities with many thousands of keys

#### Returns

`Promise`<[`PermissionedAccount`](../wiki/types.PermissionedAccount)[]\>

▸ **getSecondaryAccounts**(`callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<[`PermissionedAccount`](../wiki/types.PermissionedAccount)[]\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### getTrustingAssets

▸ **getTrustingAssets**(): `Promise`<[`Asset`](../wiki/api.entities.Asset.Asset)[]\>

Get the list of Assets for which this Identity is a trusted claim issuer

**`Note`**

 uses the middleware

#### Returns

`Promise`<[`Asset`](../wiki/api.entities.Asset.Asset)[]\>

___

### getVenues

▸ **getVenues**(): `Promise`<[`Venue`](../wiki/api.entities.Venue.Venue)[]\>

Retrieve all Venues created by this Identity

**`Note`**

 can be subscribed to

#### Returns

`Promise`<[`Venue`](../wiki/api.entities.Venue.Venue)[]\>

▸ **getVenues**(`callback`): `Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | [`SubCallback`](../wiki/types#subcallback)<[`Venue`](../wiki/api.entities.Venue.Venue)[]\> |

#### Returns

`Promise`<[`UnsubCallback`](../wiki/types#unsubcallback)\>

___

### hasRole

▸ **hasRole**(`role`): `Promise`<`boolean`\>

Check whether this Identity possesses the specified Role

#### Parameters

| Name | Type |
| :------ | :------ |
| `role` | [`Role`](../wiki/types#role) |

#### Returns

`Promise`<`boolean`\>

___

### hasRoles

▸ **hasRoles**(`roles`): `Promise`<`boolean`\>

Check whether this Identity possesses all specified roles

**`Deprecated`**

 in favor of `checkRoles`

#### Parameters

| Name | Type |
| :------ | :------ |
| `roles` | [`Role`](../wiki/types#role)[] |

#### Returns

`Promise`<`boolean`\>

___

### hasValidCdd

▸ **hasValidCdd**(): `Promise`<`boolean`\>

Check whether this Identity has a valid CDD claim

#### Returns

`Promise`<`boolean`\>

___

### isCddProvider

▸ **isCddProvider**(): `Promise`<`boolean`\>

Check whether this Identity is a CDD provider

#### Returns

`Promise`<`boolean`\>

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

### isGcMember

▸ **isGcMember**(): `Promise`<`boolean`\>

Check whether this Identity is Governance Committee member

#### Returns

`Promise`<`boolean`\>

___

### toHuman

▸ **toHuman**(): `string`

Return the Identity's DID

#### Returns

`string`

#### Overrides

[Entity](../wiki/api.entities.Entity.Entity).[toHuman](../wiki/api.entities.Entity.Entity#tohuman)

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
