# MappedEntityCollectionSuperAreasInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
**world_map_id** | **number** | World-map context supplied on super-area records. | [optional] [default to undefined]
**areas** | [**Array&lt;CombatReference&gt;**](CombatReference.md) | Child area references supplied on super-area records. | [optional] [default to undefined]
**level** | **number** | Suggested geographic difficulty level supplied on subarea records. Not a monster grade or the level of every monster there. | [optional] [default to undefined]
**dungeon_id** | **number** | Dungeon association when supplied by the subarea data. | [optional] [default to undefined]
**maps** | [**Array&lt;WorldMapReference&gt;**](WorldMapReference.md) | Map membership supplied on subarea records. Does not imply a spawn on every map. | [optional] [default to undefined]
**super_area** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**area** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**subareas** | [**Array&lt;CombatReference&gt;**](CombatReference.md) |  | [optional] [default to undefined]
**monsters** | [**Array&lt;CombatReference&gt;**](CombatReference.md) |  | [optional] [default to undefined]

## Example

```typescript
import { MappedEntityCollectionSuperAreasInner } from 'dofusdude-ts';

const instance: MappedEntityCollectionSuperAreasInner = {
    ankama_id,
    name,
    image_urls,
    world_map_id,
    areas,
    level,
    dungeon_id,
    maps,
    super_area,
    area,
    subareas,
    monsters,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
