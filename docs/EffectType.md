# EffectType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**is_active** | **boolean** | Affects target or source actively. | [optional] [default to undefined]
**is_meta** | **boolean** | true if a type is generated from the Api instead of Ankama. In that case, always prefer showing the templated string and omit everything else. The \&quot;name\&quot; field will have an english description of the meta type. An example for such effects are class sets effects. | [optional] [default to undefined]

## Example

```typescript
import { EffectType } from 'dofusdude-ts';

const instance: EffectType = {
    id,
    name,
    is_active,
    is_meta,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
