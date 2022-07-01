# Interface: PercentageTransferRestriction

[types](../wiki/types).PercentageTransferRestriction

## Hierarchy

- `TransferRestrictionBase`

  ↳ **`PercentageTransferRestriction`**

## Table of contents

### Properties

- [exemptedIds](../wiki/types.PercentageTransferRestriction#exemptedids)
- [percentage](../wiki/types.PercentageTransferRestriction#percentage)

## Properties

### exemptedIds

• `Optional` **exemptedIds**: `string`[]

array of Scope/Identity IDs that are exempted from the Restriction

**`note`** if the Asset requires investor uniqueness, Scope IDs are used. Otherwise, we use Identity IDs. More on Scope IDs and investor uniqueness
  [here](https://developers.polymesh.network/introduction/identity#polymesh-unique-identity-system-puis) and
  [here](https://developers.polymesh.network/polymesh-docs/primitives/confidential-identity)

#### Inherited from

TransferRestrictionBase.exemptedIds

#### Defined in

[types/index.ts:1245](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/types/index.ts#L1245)

___

### percentage

• **percentage**: `BigNumber`

maximum percentage (0-100) of the total supply of the Asset that can be held by a single investor at once

#### Defined in

[types/index.ts:1256](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/types/index.ts#L1256)
