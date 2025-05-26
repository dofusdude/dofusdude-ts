# ConditionNode


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_operand** | **boolean** | always \&quot;true\&quot; for the leaf of a tree | [optional] [default to true]
**relation** | **string** | \&quot;and\&quot;, \&quot;or\&quot; | [optional] [default to 'and']
**children** | [**Array&lt;ConditionNode | null&gt;**](ConditionNode.md) |  | [optional] [default to undefined]
**condition** | [**Condition**](Condition.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ConditionNode } from 'dofusdude-ts';

const instance: ConditionNode = {
    is_operand,
    relation,
    children,
    condition,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
