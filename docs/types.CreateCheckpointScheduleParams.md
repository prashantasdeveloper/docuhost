# Interface: CreateCheckpointScheduleParams

[types](../wiki/types).CreateCheckpointScheduleParams

## Table of contents

### Properties

- [period](../wiki/types.CreateCheckpointScheduleParams#period)
- [repetitions](../wiki/types.CreateCheckpointScheduleParams#repetitions)
- [start](../wiki/types.CreateCheckpointScheduleParams#start)

## Properties

### period

• **period**: ``null`` \| [`CalendarPeriod`](../wiki/types.CalendarPeriod)

The cadence with which to make Checkpoints.

**`note`** A null value indicates to create only one Checkpoint, regardless of repetitions specified. This can be used to schedule the creation of a Checkpoint in the future

#### Defined in

[api/procedures/types.ts:397](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L397)

___

### repetitions

• **repetitions**: ``null`` \| `BigNumber`

The number of snapshots to take. A null value indicates snapshots should be made indefinitely

#### Defined in

[api/procedures/types.ts:401](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L401)

___

### start

• **start**: ``null`` \| `Date`

The date from which to begin creating snapshots. A null value indicates immediately

#### Defined in

[api/procedures/types.ts:392](https://github.com/PolymathNetwork/polymesh-sdk/blob/c6fe1be3/src/api/procedures/types.ts#L392)
