# MappedEntityCollectionMonstersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
**race** | [**MonsterRace**](MonsterRace.md) |  | [default to undefined]
**grades** | [**Array&lt;MonsterGrade&gt;**](MonsterGrade.md) | Variants of this monster. Each has its own combat level, statistics and assigned spells. The monster grade number is not a spell grade number or combat level. | [default to undefined]
**spawn_locations** | [**Array&lt;MonsterSpawnLocation&gt;**](MonsterSpawnLocation.md) | Known spawn subareas and their geographic parents. This is not live population data or a per-map spawn probability. Maps listed within a subarea are not guaranteed individual spawn points. | [default to undefined]
**drops** | [**Array&lt;MonsterDrop&gt;**](MonsterDrop.md) |  | [default to undefined]
**global_drops** | [**Array&lt;MonsterGlobalDrop&gt;**](MonsterGlobalDrop.md) |  | [optional] [default to undefined]
**appearance** | [**ClassAppearance**](ClassAppearance.md) |  | [optional] [default to undefined]
**is_bounty** | **boolean** |  | [optional] [default to undefined]
**corresponding_mini_boss** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**summon_cost** | **number** |  | [optional] [default to undefined]
**speed_adjust** | **number** |  | [optional] [default to undefined]
**scale_grade_reference** | **number** |  | [optional] [default to undefined]
**achievements** | [**Array&lt;CombatReference&gt;**](CombatReference.md) |  | [optional] [default to undefined]
**souls** | **Array&lt;{ [key: string]: any; }&gt;** |  | [optional] [default to undefined]
**characteristic_ratios** | **Array&lt;Array&lt;number&gt;&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { MappedEntityCollectionMonstersInner } from 'dofusdude-ts';

const instance: MappedEntityCollectionMonstersInner = {
    ankama_id,
    name,
    image_urls,
    race,
    grades,
    spawn_locations,
    drops,
    global_drops,
    appearance,
    is_bounty,
    corresponding_mini_boss,
    summon_cost,
    speed_adjust,
    scale_grade_reference,
    achievements,
    souls,
    characteristic_ratios,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
