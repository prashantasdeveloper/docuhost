# Interface: CreateAssetWithTickerParams

[types](../wiki/types).CreateAssetWithTickerParams

## Hierarchy

- [`CreateAssetParams`](../wiki/types.CreateAssetParams)

  ↳ **`CreateAssetWithTickerParams`**

## Table of contents

### Properties

- [assetType](../wiki/types.CreateAssetWithTickerParams#assettype)
- [documents](../wiki/types.CreateAssetWithTickerParams#documents)
- [fundingRound](../wiki/types.CreateAssetWithTickerParams#fundinground)
- [initialSupply](../wiki/types.CreateAssetWithTickerParams#initialsupply)
- [isDivisible](../wiki/types.CreateAssetWithTickerParams#isdivisible)
- [name](../wiki/types.CreateAssetWithTickerParams#name)
- [requireInvestorUniqueness](../wiki/types.CreateAssetWithTickerParams#requireinvestoruniqueness)
- [securityIdentifiers](../wiki/types.CreateAssetWithTickerParams#securityidentifiers)
- [ticker](../wiki/types.CreateAssetWithTickerParams#ticker)

## Properties

### assetType

• **assetType**: `string`

type of security that the Asset represents (i.e. Equity, Debt, Commodity, etc). Common values are included in the
  [KnownAssetType](../wiki/types.KnownAssetType) enum, but custom values can be used as well. Custom values must be registered on-chain the first time
  they're used, requiring an additional transaction. They aren't tied to a specific Asset

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[assetType](../wiki/types.CreateAssetParams#assettype)

#### Defined in

[api/procedures/types.ts:172](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L172)

___

### documents

• `Optional` **documents**: [`AssetDocument`](../wiki/types.AssetDocument)[]

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[documents](../wiki/types.CreateAssetParams#documents)

#### Defined in

[api/procedures/types.ts:181](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L181)

___

### fundingRound

• `Optional` **fundingRound**: `string`

(optional) funding round in which the Asset currently is (Series A, Series B, etc)

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[fundingRound](../wiki/types.CreateAssetParams#fundinground)

#### Defined in

[api/procedures/types.ts:180](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L180)

___

### initialSupply

• `Optional` **initialSupply**: `BigNumber`

amount of Asset tokens that will be minted on creation (optional, default doesn't mint)

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[initialSupply](../wiki/types.CreateAssetParams#initialsupply)

#### Defined in

[api/procedures/types.ts:162](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L162)

___

### isDivisible

• **isDivisible**: `boolean`

whether a single Asset token can be divided into decimal parts

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[isDivisible](../wiki/types.CreateAssetParams#isdivisible)

#### Defined in

[api/procedures/types.ts:166](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L166)

___

### name

• **name**: `string`

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[name](../wiki/types.CreateAssetParams#name)

#### Defined in

[api/procedures/types.ts:158](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L158)

___

### requireInvestorUniqueness

• **requireInvestorUniqueness**: `boolean`

whether this asset requires investors to have a Investor Uniqueness Claim in order
  to hold it. More information about Investor Uniqueness and PUIS [here](https://developers.polymesh.live/introduction/identity#polymesh-unique-identity-system-puis)

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[requireInvestorUniqueness](../wiki/types.CreateAssetParams#requireinvestoruniqueness)

#### Defined in

[api/procedures/types.ts:186](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L186)

___

### securityIdentifiers

• `Optional` **securityIdentifiers**: [`SecurityIdentifier`](../wiki/types.SecurityIdentifier)[]

array of domestic or international alphanumeric security identifiers for the Asset (ISIN, CUSIP, FIGI, etc)

#### Inherited from

[CreateAssetParams](../wiki/types.CreateAssetParams).[securityIdentifiers](../wiki/types.CreateAssetParams#securityidentifiers)

#### Defined in

[api/procedures/types.ts:176](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L176)

___

### ticker

• **ticker**: `string`

#### Defined in

[api/procedures/types.ts:190](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L190)
