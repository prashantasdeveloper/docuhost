# Interface: HumanReadable

[api/entities/CorporateAction](../wiki/api.entities.CorporateAction).HumanReadable

## Hierarchy

- **`HumanReadable`**

  ↳ [`HumanReadable`](../wiki/api.entities.DividendDistribution.HumanReadable)

## Table of contents

### Properties

- [declarationDate](../wiki/api.entities.CorporateAction.HumanReadable#declarationdate)
- [defaultTaxWithholding](../wiki/api.entities.CorporateAction.HumanReadable#defaulttaxwithholding)
- [description](../wiki/api.entities.CorporateAction.HumanReadable#description)
- [id](../wiki/api.entities.CorporateAction.HumanReadable#id)
- [targets](../wiki/api.entities.CorporateAction.HumanReadable#targets)
- [taxWithholdings](../wiki/api.entities.CorporateAction.HumanReadable#taxwithholdings)
- [ticker](../wiki/api.entities.CorporateAction.HumanReadable#ticker)

## Properties

### declarationDate

• **declarationDate**: `string`

#### Defined in

[api/entities/CorporateAction.ts:24](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/CorporateAction.ts#L24)

___

### defaultTaxWithholding

• **defaultTaxWithholding**: `string`

#### Defined in

[api/entities/CorporateAction.ts:27](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/CorporateAction.ts#L27)

___

### description

• **description**: `string`

#### Defined in

[api/entities/CorporateAction.ts:25](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/CorporateAction.ts#L25)

___

### id

• **id**: `string`

#### Defined in

[api/entities/CorporateAction.ts:22](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/CorporateAction.ts#L22)

___

### targets

• **targets**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `identities` | `string`[] |
| `treatment` | [`TargetTreatment`](../wiki/api.entities.CorporateActionBase.types.TargetTreatment) |

#### Defined in

[api/entities/CorporateAction.ts:26](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/CorporateAction.ts#L26)

___

### taxWithholdings

• **taxWithholdings**: { `identity`: `string` ; `percentage`: `string`  }[]

#### Defined in

[api/entities/CorporateAction.ts:28](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/CorporateAction.ts#L28)

___

### ticker

• **ticker**: `string`

#### Defined in

[api/entities/CorporateAction.ts:23](https://github.com/PolymathNetwork/polymesh-sdk/blob/c37bc05d/src/api/entities/CorporateAction.ts#L23)
