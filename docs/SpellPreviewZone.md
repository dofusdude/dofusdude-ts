# SpellPreviewZone

Client preview binding. Activation criteria and display geometry serve a different purpose from an effect\'s zone.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**activation_mask** | [**TargetMask**](TargetMask.md) |  | [optional] [default to undefined]
**caster_mask** | [**TargetMask**](TargetMask.md) |  | [optional] [default to undefined]
**hidden** | **boolean** |  | [optional] [default to undefined]
**activation_zone** | [**EffectZone**](EffectZone.md) |  | [optional] [default to undefined]
**display_zone** | [**EffectZone**](EffectZone.md) |  | [optional] [default to undefined]

## Example

```typescript
import { SpellPreviewZone } from 'dofusdude-ts';

const instance: SpellPreviewZone = {
    ankama_id,
    activation_mask,
    caster_mask,
    hidden,
    activation_zone,
    display_zone,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
