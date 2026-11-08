# TargetMask


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**raw** | **string** | Original game mask retained for lossless debugging. | [default to undefined]
**logic** | **string** |  | [optional] [default to undefined]
**conditions** | [**Array&lt;CombatCondition&gt;**](CombatCondition.md) |  | [optional] [default to undefined]
**selectors** | [**Array&lt;TargetSelector&gt;**](TargetSelector.md) |  | [default to undefined]

## Example

```typescript
import { TargetMask } from 'dofusdude-ts';

const instance: TargetMask = {
    raw,
    logic,
    conditions,
    selectors,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
