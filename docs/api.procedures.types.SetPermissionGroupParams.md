# Interface: SetPermissionGroupParams

[api/procedures/types](../wiki/api.procedures.types).SetPermissionGroupParams

This procedure can be called with:
  - An Asset's existing Custom Permission Group. The Identity will be assigned as an Agent of that Group for that Asset
  - A Known Permission Group and an Asset. The Identity will be assigned as an Agent of that Group for that Asset
  - A set of Transaction Permissions and an Asset. If there is no Custom Permission Group with those permissions, a Custom Permission Group will be created for that Asset with those permissions, and
    the Identity will be assigned as an Agent of that Group for that Asset. Otherwise, the existing Group will be used
  - An array of [Transaction Groups](../wiki/types.TxGroup) that represent a set of permissions. If there is no Custom Permission Group with those permissions, a Custom Permission Group will be created with those permissions, and
    the Identity will be assigned as an Agent of that Group for that Asset. Otherwise, the existing Group will be used

## Table of contents

### Properties

- [group](../wiki/api.procedures.types.SetPermissionGroupParams#group)

## Properties

### group

• **group**: [`KnownPermissionGroup`](../wiki/api.entities.KnownPermissionGroup.KnownPermissionGroup) \| [`CustomPermissionGroup`](../wiki/api.entities.CustomPermissionGroup.CustomPermissionGroup) \| [`TransactionsParams`](../wiki/api.procedures.types.TransactionsParams) \| [`TxGroupParams`](../wiki/api.procedures.types.TxGroupParams)

#### Defined in

[api/procedures/types.ts:766](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L766)