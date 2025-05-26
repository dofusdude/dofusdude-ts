# ConditionRelation



## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_operand** | **boolean** | always \&quot;false\&quot; for relations | [optional] [default to false]
**relation** | **string** | \&quot;and\&quot;, \&quot;or\&quot; | [optional] [default to 'and']
**children** | [**Array&lt;ConditionNode | null&gt;**](ConditionNode.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ConditionRelation } from 'dofusdude-ts';

const instance: ConditionRelation = {
    is_operand,
    relation,
    children,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
