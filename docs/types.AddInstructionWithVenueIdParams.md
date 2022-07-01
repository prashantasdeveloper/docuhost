# Interface: AddInstructionWithVenueIdParams

[types](../wiki/types).AddInstructionWithVenueIdParams

## Hierarchy

- [`AddInstructionParams`](../wiki/types.AddInstructionParams)

  ↳ **`AddInstructionWithVenueIdParams`**

## Table of contents

### Properties

- [endBlock](../wiki/types.AddInstructionWithVenueIdParams#endblock)
- [legs](../wiki/types.AddInstructionWithVenueIdParams#legs)
- [tradeDate](../wiki/types.AddInstructionWithVenueIdParams#tradedate)
- [valueDate](../wiki/types.AddInstructionWithVenueIdParams#valuedate)
- [venueId](../wiki/types.AddInstructionWithVenueIdParams#venueid)

## Properties

### endBlock

• `Optional` **endBlock**: `BigNumber`

block at which the Instruction will be executed automatically (optional, the Instruction will be executed when all participants have authorized it if not supplied)

#### Inherited from

[AddInstructionParams](../wiki/types.AddInstructionParams).[endBlock](../wiki/types.AddInstructionParams#endblock)

#### Defined in

[api/procedures/types.ts:291](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L291)

___

### legs

• **legs**: { `amount`: `BigNumber` ; `asset`: `string` \| [`Asset`](../wiki/api.entities.Asset.Asset) ; `from`: [`PortfolioLike`](../wiki/types#portfoliolike) ; `to`: [`PortfolioLike`](../wiki/types#portfoliolike)  }[]

array of Asset movements (amount, from, to, asset)

#### Inherited from

[AddInstructionParams](../wiki/types.AddInstructionParams).[legs](../wiki/types.AddInstructionParams#legs)

#### Defined in

[api/procedures/types.ts:274](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L274)

___

### tradeDate

• `Optional` **tradeDate**: `Date`

date at which the trade was agreed upon (optional, for off chain trades)

#### Inherited from

[AddInstructionParams](../wiki/types.AddInstructionParams).[tradeDate](../wiki/types.AddInstructionParams#tradedate)

#### Defined in

[api/procedures/types.ts:283](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L283)

___

### valueDate

• `Optional` **valueDate**: `Date`

date at which the trade was executed (optional, for off chain trades)

#### Inherited from

[AddInstructionParams](../wiki/types.AddInstructionParams).[valueDate](../wiki/types.AddInstructionParams#valuedate)

#### Defined in

[api/procedures/types.ts:287](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L287)

___

### venueId

• **venueId**: `BigNumber`

#### Defined in

[api/procedures/types.ts:302](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L302)
