# MappedEntityCollectionSuperAreasInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
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
    super_area,
    area,
    subareas,
    monsters,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
