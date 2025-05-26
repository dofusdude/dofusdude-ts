# ListItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**type** | [**TranslatedId**](TranslatedId.md) |  | [optional] [default to undefined]
**level** | **number** |  | [optional] [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
**recipe** | [**Array&lt;Recipe&gt;**](Recipe.md) |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**conditions** | [**ConditionNode**](ConditionNode.md) |  | [optional] [default to undefined]
**effects** | [**Array&lt;Effect&gt;**](Effect.md) |  | [optional] [default to undefined]
**is_weapon** | **boolean** |  | [optional] [default to undefined]
**pods** | **number** |  | [optional] [default to undefined]
**parent_set** | [**TranslatedId**](TranslatedId.md) |  | [optional] [default to undefined]
**critical_hit_probability** | **number** |  | [optional] [default to undefined]
**critical_hit_bonus** | **number** |  | [optional] [default to undefined]
**max_cast_per_turn** | **number** |  | [optional] [default to undefined]
**ap_cost** | **number** |  | [optional] [default to undefined]
**range** | [**Range**](Range.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ListItem } from 'dofusdude-ts';

const instance: ListItem = {
    ankama_id,
    name,
    type,
    level,
    image_urls,
    recipe,
    description,
    conditions,
    effects,
    is_weapon,
    pods,
    parent_set,
    critical_hit_probability,
    critical_hit_bonus,
    max_cast_per_turn,
    ap_cost,
    range,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
