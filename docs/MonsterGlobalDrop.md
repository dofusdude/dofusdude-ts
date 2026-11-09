# MonsterGlobalDrop

A separate global-drop entry with a base percentage range. It is not the per-monster-grade rates table and does not by itself define a final player-specific drop chance.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**has_conditions** | **boolean** |  | [optional] [default to undefined]
**item** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**min_percent** | **number** |  | [default to undefined]
**max_percent** | **number** |  | [default to undefined]
**condition** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**alteration_id** | **number** |  | [optional] [default to undefined]
**disable_drop_modifier** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { MonsterGlobalDrop } from 'dofusdude-ts';

const instance: MonsterGlobalDrop = {
    has_conditions,
    item,
    min_percent,
    max_percent,
    condition,
    alteration_id,
    disable_drop_modifier,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
