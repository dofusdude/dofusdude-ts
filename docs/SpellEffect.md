# SpellEffect

One normal or critical effect of a particular spell grade. Its zone defines where it applies, target_mask defines eligible targets and triggers defines activation events. Templated text is for display, not a formula to parse.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **string** | Localized effect category, such as Air damage. This is not a spell ID or a structured game reference. | [optional] [default to undefined]
**min** | **number** |  | [optional] [default to undefined]
**max** | **number** |  | [optional] [default to undefined]
**duration** | **number** | Effect duration in fight turns as represented by the source. Not a real-time duration in seconds. | [optional] [default to undefined]
**delay** | **number** | Delay before the effect in fight turns as represented by the source. | [optional] [default to undefined]
**random** | **number** | Source random-selection value. Do not interpret it as a percentage without the effect\&#39;s selection rules. | [optional] [default to undefined]
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
**templated** | **string** | Localized effect text suitable for display. Numeric effect properties remain available separately. | [optional] [default to undefined]

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
