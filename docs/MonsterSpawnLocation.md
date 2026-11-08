# MonsterSpawnLocation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subarea** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**area** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**super_area** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**subarea_maps** | [**Array&lt;MonsterSpawnLocationSubareaMapsInner&gt;**](MonsterSpawnLocationSubareaMapsInner.md) |  | [default to undefined]
**preferred** | **boolean** | Whether the game marks this as the monster\&#39;s preferred subarea. | [default to undefined]

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
