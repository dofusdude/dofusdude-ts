# MappedEntityCollectionClassesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**gameplay_description** | **string** |  | [optional] [default to undefined]
**complexity** | **number** |  | [optional] [default to undefined]
**sort_index** | **number** |  | [optional] [default to undefined]
**creature_bones_id** | **number** |  | [optional] [default to undefined]
**roles** | **Array&lt;{ [key: string]: any; }&gt;** |  | [optional] [default to undefined]
**characteristic_costs** | **{ [key: string]: Array&lt;ClassCharacteristicCostsValueInner&gt;; }** | Characteristic point-cost tiers keyed by characteristic name. | [optional] [default to undefined]
**looks** | [**ClassLooks**](ClassLooks.md) |  | [default to undefined]
**spells** | [**Array&lt;Spell&gt;**](Spell.md) | Fully mapped class spells, including levels, effects, targeting, and zones. | [default to undefined]

## Example

```typescript
import { MappedEntityCollectionClassesInner } from 'dofusdude-ts';

const instance: MappedEntityCollectionClassesInner = {
    ankama_id,
    name,
    image_urls,
    description,
    gameplay_description,
    complexity,
    sort_index,
    creature_bones_id,
    roles,
    characteristic_costs,
    looks,
    spells,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
