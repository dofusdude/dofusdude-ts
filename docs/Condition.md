# Condition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**operator** | **string** | Comparison to apply to the interpreted requirement value. | [optional] [default to undefined]
**int_value** | **number** |  | [optional] [default to undefined]
**element** | [**TranslatedId**](TranslatedId.md) |  | [optional] [default to undefined]
**kind** | **string** | Interpreted requirement category, such as profession_level or item_received_age. Use this with the operator, values and references rather than decoding original condition tokens. | [optional] [default to undefined]
**unit** | **string** | Unit associated with the requirement value when the interpreted condition supplies one. | [optional] [default to undefined]
**quantity** | **number** |  | [optional] [default to undefined]
**string_value** | **string** |  | [optional] [default to undefined]
**value_label** | **string** |  | [optional] [default to undefined]
**reference** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**secondary_reference** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Condition } from 'dofusdude-ts';

const instance: Condition = {
    operator,
    int_value,
    element,
    kind,
    unit,
    quantity,
    string_value,
    value_label,
    reference,
    secondary_reference,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
