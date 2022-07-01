# Interface: AddInstructionParams

[api/procedures/types](../wiki/api.procedures.types).AddInstructionParams

## Hierarchy

- **`AddInstructionParams`**

  ↳ [`AddInstructionWithVenueIdParams`](../wiki/api.procedures.types.AddInstructionWithVenueIdParams)

## Table of contents

### Properties

- [endBlock](../wiki/api.procedures.types.AddInstructionParams#endblock)
- [legs](../wiki/api.procedures.types.AddInstructionParams#legs)
- [tradeDate](../wiki/api.procedures.types.AddInstructionParams#tradedate)
- [valueDate](../wiki/api.procedures.types.AddInstructionParams#valuedate)

## Properties

### endBlock

• `Optional` **endBlock**: `BigNumber`

block at which the Instruction will be executed automatically (optional, the Instruction will be executed when all participants have authorized it if not supplied)

#### Defined in

[api/procedures/types.ts:291](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L291)

___

### legs

• **legs**: { `amount`: `BigNumber` ; `asset`: `string` \| [`Asset`](../wiki/api.entities.Asset.Asset) ; `from`: [`PortfolioLike`](../wiki/types#portfoliolike) ; `to`: [`PortfolioLike`](../wiki/types#portfoliolike)  }[]

array of Asset movements (amount, from, to, asset)

#### Defined in

[api/procedures/types.ts:274](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L274)

___

### tradeDate

• `Optional` **tradeDate**: `Date`

date at which the trade was agreed upon (optional, for off chain trades)

#### Defined in

[api/procedures/types.ts:283](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L283)

___

### valueDate

• `Optional` **valueDate**: `Date`

date at which the trade was executed (optional, for off chain trades)

#### Defined in

[api/procedures/types.ts:287](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L287)
