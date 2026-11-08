# TargetSelector


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**kind** | **string** | Human-readable target category or relationship. | [optional] [default to undefined]
**code** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**subject** | **string** |  | [optional] [default to undefined]
**negated** | **boolean** |  | [optional] [default to undefined]
**reference** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**conditions** | [**Array&lt;CombatCondition&gt;**](CombatCondition.md) |  | [optional] [default to undefined]

## Example

```typescript
import { TargetSelector } from 'dofusdude-ts';

const instance: TargetSelector = {
    kind,
    code,
    name,
    description,
    subject,
    negated,
    reference,
    conditions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
