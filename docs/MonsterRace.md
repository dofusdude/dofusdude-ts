# MonsterRace

Monster taxonomy. Race is the monster\'s family and super_race is the broader grouping. Neither is a playable class or a monster grade.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**super_race** | [**CombatReference**](CombatReference.md) |  | [default to undefined]

## Example

```typescript
import { MonsterRace } from 'dofusdude-ts';

const instance: MonsterRace = {
    ankama_id,
    name,
    super_race,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
