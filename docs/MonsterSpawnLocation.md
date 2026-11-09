# MonsterSpawnLocation

Known spawn subarea with its parent area, super-area and map membership. Does not assert a spawn on each listed map and does not include spawn probabilities.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subarea** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**area** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**super_area** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**subarea_maps** | [**Array&lt;MonsterSpawnLocationSubareaMapsInner&gt;**](MonsterSpawnLocationSubareaMapsInner.md) | Maps belonging to the referenced subarea. Map membership alone is not proof that the monster spawns on a particular map. | [default to undefined]
**preferred** | **boolean** | Whether the source marks this as a preferred subarea. A preference flag, not a spawn percentage or guarantee of presence. | [default to undefined]

## Example

```typescript
import { MonsterSpawnLocation } from 'dofusdude-ts';

const instance: MonsterSpawnLocation = {
    subarea,
    area,
    super_area,
    subarea_maps,
    preferred,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
