# SpellScriptUsage

Resolved client-side spell script binding, including target selection and areas.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**script_id** | **number** |  | [optional] [default to undefined]
**order** | **number** |  | [optional] [default to undefined]
**random** | **number** |  | [optional] [default to undefined]
**random_group** | **number** |  | [optional] [default to undefined]
**sequence_group** | **number** |  | [optional] [default to undefined]
**activation_mask** | [**TargetMask**](TargetMask.md) |  | [optional] [default to undefined]
**caster_mask** | [**TargetMask**](TargetMask.md) |  | [optional] [default to undefined]
**target_mask** | [**TargetMask**](TargetMask.md) |  | [optional] [default to undefined]
**activation_zone** | [**EffectZone**](EffectZone.md) |  | [optional] [default to undefined]
**target_zone** | [**EffectZone**](EffectZone.md) |  | [optional] [default to undefined]
**condition** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**targets_affected_concurrently** | **boolean** |  | [optional] [default to undefined]
**target_treated_as_caster** | **boolean** |  | [optional] [default to undefined]
**spell_level_ids** | **Array&lt;number&gt;** | Spell-level definition IDs to which this script binding applies. Match SpellLevel.ankama_id, not Spell.ankama_id or SpellLevel.grade. | [optional] [default to undefined]

## Example

```typescript
import { SpellScriptUsage } from 'dofusdude-ts';

const instance: SpellScriptUsage = {
    ankama_id,
    script_id,
    order,
    random,
    random_group,
    sequence_group,
    activation_mask,
    caster_mask,
    target_mask,
    activation_zone,
    target_zone,
    condition,
    targets_affected_concurrently,
    target_treated_as_caster,
    spell_level_ids,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
