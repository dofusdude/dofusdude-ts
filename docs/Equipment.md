# Equipment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**type** | [**TranslatedId**](TranslatedId.md) |  | [optional] [default to undefined]
**is_weapon** | **boolean** |  | [optional] [default to undefined]
**level** | **number** |  | [optional] [default to undefined]
**pods** | **number** |  | [optional] [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
**effects** | [**Array&lt;Effect&gt;**](Effect.md) |  | [optional] [default to undefined]
**conditions** | [**ConditionNode**](ConditionNode.md) |  | [optional] [default to undefined]
**recipe** | [**Array&lt;Recipe&gt;**](Recipe.md) |  | [optional] [default to undefined]
**parent_set** | [**TranslatedId**](TranslatedId.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Equipment } from 'dofusdude-ts';

const instance: Equipment = {
    ankama_id,
    name,
    description,
    type,
    is_weapon,
    level,
    pods,
    image_urls,
    effects,
    conditions,
    recipe,
    parent_set,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
