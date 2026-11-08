# MonsterSpellRelationship


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**grade** | **number** | The spell grade assigned to this monster grade. | [default to undefined]
**url** | **string** | URL for the assigned spell grade. Includes the &#x60;grade&#x60; query parameter. | [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]

## Example

```typescript
import { MonsterSpellRelationship } from 'dofusdude-ts';

const instance: MonsterSpellRelationship = {
    ankama_id,
    name,
    grade,
    url,
    image_urls,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
