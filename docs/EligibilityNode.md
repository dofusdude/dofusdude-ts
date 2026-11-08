# EligibilityNode

Client-side conditions using the v1 condition-node structure. Confirmed server-owned predicates are excluded during mapping. This is not the complete server eligibility formula, and the API does not dynamically remove fields based on interpretation status.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_operand** | **boolean** |  | [optional] [default to undefined]
**relation** | **string** |  | [optional] [default to undefined]
**children** | [**Array&lt;EligibilityNode&gt;**](EligibilityNode.md) |  | [optional] [default to undefined]
**condition** | [**EligibilityNodeCondition**](EligibilityNodeCondition.md) |  | [optional] [default to undefined]

## Example

```typescript
import { EligibilityNode } from 'dofusdude-ts';

const instance: EligibilityNode = {
    is_operand,
    relation,
    children,
    condition,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
