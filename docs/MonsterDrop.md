# MonsterDrop

A possible item drop with base rates indexed by monster grade. Final player-specific chances also depend on conditions and game modifiers.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**item** | [**CombatReference**](CombatReference.md) |  | [default to undefined]
**rates_percent** | [**Array&lt;MonsterDropRatesPercentInner&gt;**](MonsterDropRatesPercentInner.md) | Base drop percentages indexed by MonsterGrade.grade, not spell grade or array position. A value of 5 means 5 percent, not 0.05 percent. These are not spawn percentages. | [default to undefined]
**has_conditions** | **boolean** | The source reports restrictions. Can be true without a complete client-side condition tree because server-only predicates are not exposed. | [default to undefined]
**drop_id** | **number** |  | [optional] [default to undefined]
**count** | **number** |  | [optional] [default to undefined]
**condition** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**hidden_if_invalid_conditions** | **boolean** |  | [optional] [default to undefined]
**disable_drop_modifier** | **boolean** |  | [optional] [default to undefined]
**specific_coefficients** | **Array&lt;{ [key: string]: any; }&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { MonsterDrop } from 'dofusdude-ts';

const instance: MonsterDrop = {
    item,
    rates_percent,
    has_conditions,
    drop_id,
    count,
    condition,
    hidden_if_invalid_conditions,
    disable_drop_modifier,
    specific_coefficients,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
