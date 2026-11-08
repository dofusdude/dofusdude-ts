# SpellEffect


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**min** | **number** |  | [optional] [default to undefined]
**max** | **number** |  | [optional] [default to undefined]
**duration** | **number** |  | [optional] [default to undefined]
**delay** | **number** |  | [optional] [default to undefined]
**random** | **number** |  | [optional] [default to undefined]
**group** | **number** |  | [optional] [default to undefined]
**dispellable** | **number** |  | [optional] [default to undefined]
**effect_uid** | **number** | Stable identifier of this concrete effect instance. | [optional] [default to undefined]
**target_id** | **number** |  | [optional] [default to undefined]
**triggered_duration** | **number** |  | [optional] [default to undefined]
**display_zero** | **boolean** |  | [optional] [default to undefined]
**modifier** | **number** |  | [optional] [default to undefined]
**zone** | [**EffectZone**](EffectZone.md) |  | [optional] [default to undefined]
**target_mask** | [**TargetMask**](TargetMask.md) |  | [optional] [default to undefined]
**triggers** | [**SpellTriggers**](SpellTriggers.md) |  | [optional] [default to undefined]
**templated** | **{ [key: string]: any; }** |  | [optional] [default to undefined]

## Example

```typescript
import { SpellEffect } from 'dofusdude-ts';

const instance: SpellEffect = {
    type,
    min,
    max,
    duration,
    delay,
    random,
    group,
    dispellable,
    effect_uid,
    target_id,
    triggered_duration,
    display_zero,
    modifier,
    zone,
    target_mask,
    triggers,
    templated,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
