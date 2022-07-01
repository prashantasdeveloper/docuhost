# Class: Subsidy

[api/entities/Subsidy](../wiki/api.entities.Subsidy).Subsidy

Represents a Subsidy relationship on chain

## Hierarchy

- [`Entity`](../wiki/api.entities.Entity.Entity)<[`UniqueIdentifiers`](../wiki/api.entities.Subsidy.UniqueIdentifiers), `HumanReadable`\>

  ↳ **`Subsidy`**

## Table of contents

### Properties

- [beneficiary](../wiki/api.entities.Subsidy.Subsidy#beneficiary)
- [subsidizer](../wiki/api.entities.Subsidy.Subsidy#subsidizer)
- [uuid](../wiki/api.entities.Subsidy.Subsidy#uuid)

### Methods

- [decreaseAllowance](../wiki/api.entities.Subsidy.Subsidy#decreaseallowance)
- [exists](../wiki/api.entities.Subsidy.Subsidy#exists)
- [getAllowance](../wiki/api.entities.Subsidy.Subsidy#getallowance)
- [increaseAllowance](../wiki/api.entities.Subsidy.Subsidy#increaseallowance)
- [isEqual](../wiki/api.entities.Subsidy.Subsidy#isequal)
- [quit](../wiki/api.entities.Subsidy.Subsidy#quit)
- [setAllowance](../wiki/api.entities.Subsidy.Subsidy#setallowance)
- [toHuman](../wiki/api.entities.Subsidy.Subsidy#tohuman)
- [generateUuid](../wiki/api.entities.Subsidy.Subsidy#generateuuid)
- [unserialize](../wiki/api.entities.Subsidy.Subsidy#unserialize)

## Properties

### beneficiary

• **beneficiary**: [`Account`](../wiki/api.entities.Account.Account)

Account whose transactions are being paid for

#### Defined in

[api/entities/Subsidy/index.ts:55](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L55)

___

### subsidizer

• **subsidizer**: [`Account`](../wiki/api.entities.Account.Account)

Account that is paying for the transactions

#### Defined in

[api/entities/Subsidy/index.ts:59](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L59)

___

### uuid

• **uuid**: `string`

#### Inherited from

[Entity](../wiki/api.entities.Entity.Entity).[uuid](../wiki/api.entities.Entity.Entity#uuid)

#### Defined in

[api/entities/Entity.ts:46](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Entity.ts#L46)

## Methods

### decreaseAllowance

▸ **decreaseAllowance**(`args`, `opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Decrease allowance for this Subsidy relationship

**`note`** Only the subsidizer is allowed to decrease the allowance

**`throws`** if the amount to decrease by is more than the existing allowance

**`note`** this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [decreaseAllowance.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Pick`<[`DecreaseAllowanceParams`](../wiki/types.DecreaseAllowanceParams), ``"allowance"``\> |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

#### Defined in

[api/entities/Subsidy/index.ts:180](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L180)

___

### exists

▸ **exists**(): `Promise`<`boolean`\>

Determine whether this Subsidy relationship exists on chain

#### Returns

`Promise`<`boolean`\>

#### Overrides

[Entity](../wiki/api.entities.Entity.Entity).[exists](../wiki/api.entities.Entity.Entity#exists)

#### Defined in

[api/entities/Subsidy/index.ts:187](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L187)

___

### getAllowance

▸ **getAllowance**(): `Promise`<`BigNumber`\>

Get amount of POLYX subsidized for this Subsidy relationship

**`throws`** if the Subsidy does not exist

#### Returns

`Promise`<`BigNumber`\>

#### Defined in

[api/entities/Subsidy/index.ts:206](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L206)

___

### increaseAllowance

▸ **increaseAllowance**(`args`, `opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Increase allowance for this Subsidy relationship

**`note`** Only the subsidizer is allowed to increase the allowance

**`note`** this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [increaseAllowance.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Pick`<[`IncreaseAllowanceParams`](../wiki/types.IncreaseAllowanceParams), ``"allowance"``\> |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

#### Defined in

[api/entities/Subsidy/index.ts:166](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L166)

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

#### Defined in

[api/entities/Entity.ts:61](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Entity.ts#L61)

___

### quit

▸ **quit**(`opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Terminate this Subsidy relationship. The beneficiary Account will be forced to pay for their own transactions

**`note`** both the beneficiary and the subsidizer are allowed to unilaterally quit the Subsidy

**`note`** this method is of type [NoArgsProcedureMethod](../wiki/types.NoArgsProcedureMethod), which means you can call [quit.checkAuthorization](../wiki/types.NoArgsProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

#### Defined in

[api/entities/Subsidy/index.ts:140](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L140)

___

### setAllowance

▸ **setAllowance**(`args`, `opts?`): `Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

Set allowance for this Subsidy relationship

**`note`** Only the subsidizer is allowed to set the allowance

**`throws`** if the allowance to set is equal to the current allowance

**`note`** this method is of type [ProcedureMethod](../wiki/types.ProcedureMethod), which means you can call [setAllowance.checkAuthorization](../wiki/types.ProcedureMethod#checkauthorization)
  on it to see whether the signing Account and Identity have the required roles and permissions to run it

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Pick`<[`SetAllowanceParams`](../wiki/types.SetAllowanceParams), ``"allowance"``\> |
| `opts?` | [`ProcedureOpts`](../wiki/types.ProcedureOpts) |

#### Returns

`Promise`<`TransactionQueue`<`void`, `void`, `unknown`[][]\>\>

#### Defined in

[api/entities/Subsidy/index.ts:154](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L154)

___

### toHuman

▸ **toHuman**(): [`UniqueIdentifiers`](../wiki/api.entities.Subsidy.UniqueIdentifiers)

Return the Subsidy's static data

#### Returns

[`UniqueIdentifiers`](../wiki/api.entities.Subsidy.UniqueIdentifiers)

#### Overrides

[Entity](../wiki/api.entities.Entity.Entity).[toHuman](../wiki/api.entities.Entity.Entity#tohuman)

#### Defined in

[api/entities/Subsidy/index.ts:228](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Subsidy/index.ts#L228)

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

#### Defined in

[api/entities/Entity.ts:14](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Entity.ts#L14)

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

#### Defined in

[api/entities/Entity.ts:23](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/entities/Entity.ts#L23)
