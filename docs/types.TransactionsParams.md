# Interface: TransactionsParams

[types](../wiki/types).TransactionsParams

## Hierarchy

- [`AssetBase`](../wiki/types.AssetBase)

  ↳ **`TransactionsParams`**

## Table of contents

### Properties

- [asset](../wiki/types.TransactionsParams#asset)
- [transactions](../wiki/types.TransactionsParams#transactions)

## Properties

### asset

• **asset**: `string` \| [`Asset`](../wiki/api.entities.Asset.Asset)

Asset over which the Identity will be granted permissions

#### Inherited from

[AssetBase](../wiki/types.AssetBase).[asset](../wiki/types.AssetBase#asset)

#### Defined in

[api/procedures/types.ts:742](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L742)

___

### transactions

• **transactions**: ``null`` \| [`TransactionPermissions`](../wiki/types.TransactionPermissions)

a null value means full permissions

#### Defined in

[api/procedures/types.ts:749](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L749)
