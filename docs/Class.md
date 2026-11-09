# Class

A playable class with its characteristics, appearance and class spell assignments.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**gameplay_description** | **string** |  | [optional] [default to undefined]
**complexity** | **number** |  | [optional] [default to undefined]
**sort_index** | **number** |  | [optional] [default to undefined]
**creature_bones_id** | **number** |  | [optional] [default to undefined]
**roles** | **Array&lt;{ [key: string]: any; }&gt;** |  | [optional] [default to undefined]
**characteristic_costs** | **{ [key: string]: Array&lt;ClassCharacteristicCostsValueInner&gt;; }** | Characteristic point-cost tiers keyed by characteristic name. | [optional] [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
**looks** | [**ClassLooks**](ClassLooks.md) |  | [default to undefined]
**spells** | [**Array&lt;Spell&gt;**](Spell.md) | Full spell definitions assigned to this playable class, including their own grades, effects and targeting. A class has no monster-grade dimension. The same spells are independently available from the spells endpoint. | [default to undefined]

## Example

```typescript
import { Class } from 'dofusdude-ts';

const instance: Class = {
    ankama_id,
    name,
    description,
    gameplay_description,
    complexity,
    sort_index,
    creature_bones_id,
    roles,
    characteristic_costs,
    image_urls,
    looks,
    spells,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
