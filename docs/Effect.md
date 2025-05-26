# Effect


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**int_minimum** | **number** | minimum int value, can be a single if ignore_int_max and no ignore_int_min | [optional] [default to undefined]
**int_maximum** | **number** | maximum int value, if not ignore_int_max and not ignore_int_min, the effect has a range value | [optional] [default to undefined]
**type** | [**EffectType**](EffectType.md) |  | [optional] [default to undefined]
**ignore_int_min** | **boolean** | ignore the int min field because the actual value is a string. For readability the templated field is the only important field in this case.  | [optional] [default to undefined]
**ignore_int_max** | **boolean** | ignore the int max field, if ignore_int_min is true, int min is a single value | [optional] [default to undefined]
**formatted** | **string** | all fields from above encoded in a single string | [optional] [default to undefined]

## Example

```typescript
import { Effect } from 'dofusdude-ts';

const instance: Effect = {
    int_minimum,
    int_maximum,
    type,
    ignore_int_min,
    ignore_int_max,
    formatted,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
