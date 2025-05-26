# EquipmentSet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**equipment_ids** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**effects** | **{ [key: string]: Array&lt;Effect&gt;; }** |  | [optional] [default to undefined]
**highest_equipment_level** | **number** |  | [optional] [default to undefined]
**contains_cosmetics** | **boolean** |  | [optional] [default to undefined]
**contains_cosmetics_only** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { EquipmentSet } from 'dofusdude-ts';

const instance: EquipmentSet = {
    ankama_id,
    name,
    equipment_ids,
    effects,
    highest_equipment_level,
    contains_cosmetics,
    contains_cosmetics_only,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
