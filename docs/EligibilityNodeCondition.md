# EligibilityNodeCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**operator** | **string** |  | [optional] [default to undefined]
**int_value** | **number** |  | [optional] [default to undefined]
**quantity** | **number** |  | [optional] [default to undefined]
**kind** | **string** | Verified semantic requirement type, for example item_received_age or profession_level. | [optional] [default to undefined]
**unit** | **string** |  | [optional] [default to undefined]
**string_value** | **string** |  | [optional] [default to undefined]
**value_label** | **string** |  | [optional] [default to undefined]
**element** | [**EligibilityNodeConditionElement**](EligibilityNodeConditionElement.md) |  | [optional] [default to undefined]
**reference** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**secondary_reference** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]

## Example

```typescript
import { EligibilityNodeCondition } from 'dofusdude-ts';

const instance: EligibilityNodeCondition = {
    operator,
    int_value,
    quantity,
    kind,
    unit,
    string_value,
    value_label,
    element,
    reference,
    secondary_reference,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
