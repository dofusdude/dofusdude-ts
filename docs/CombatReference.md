# CombatReference

A compact resolved reference, not a complete resource. Interpret the ID in the context of the containing field. IDs in different resource types can have the same numeric value without referring to the same entity.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**kind** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { CombatReference } from 'dofusdude-ts';

const instance: CombatReference = {
    ankama_id,
    name,
    kind,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
