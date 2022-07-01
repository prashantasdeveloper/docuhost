# Interface: SimplePermissions

[types](../wiki/types).SimplePermissions

This represents positive permissions (i.e. only "includes"). It is used
  for specifying procedure requirements and querying if an Account has certain
  permissions. Null values represent full permissions in that category

## Table of contents

### Properties

- [assets](../wiki/types.SimplePermissions#assets)
- [portfolios](../wiki/types.SimplePermissions#portfolios)
- [transactions](../wiki/types.SimplePermissions#transactions)

## Properties

### assets

• `Optional` **assets**: ``null`` \| [`Asset`](../wiki/api.entities.Asset.Asset)[]

list of required Asset permissions

#### Defined in

[types/index.ts:967](https://github.com/PolymathNetwork/polymesh-sdk/blob/49113a20/src/types/index.ts#L967)

___

### portfolios

• `Optional` **portfolios**: ``null`` \| ([`NumberedPortfolio`](../wiki/api.entities.NumberedPortfolio.NumberedPortfolio) \| [`DefaultPortfolio`](../wiki/api.entities.DefaultPortfolio.DefaultPortfolio))[]

#### Defined in

[types/index.ts:973](https://github.com/PolymathNetwork/polymesh-sdk/blob/49113a20/src/types/index.ts#L973)

___

### transactions

• `Optional` **transactions**: ``null`` \| [`TxTag`](../wiki/generated.types#txtag)[]

list of required Transaction permissions

#### Defined in

[types/index.ts:971](https://github.com/PolymathNetwork/polymesh-sdk/blob/49113a20/src/types/index.ts#L971)
