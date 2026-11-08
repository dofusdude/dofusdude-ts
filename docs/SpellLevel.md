# SpellLevel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**grade** | **number** |  | [optional] [default to undefined]
**ap_cost** | **number** |  | [optional] [default to undefined]
**min_range** | **number** |  | [optional] [default to undefined]
**max_range** | **number** |  | [optional] [default to undefined]
**max_cast_per_turn** | **number** |  | [optional] [default to undefined]
**max_cast_per_target** | **number** |  | [optional] [default to undefined]
**max_global_cast_per_turn** | **number** |  | [optional] [default to undefined]
**max_global_cast_per_target** | **number** |  | [optional] [default to undefined]
**min_cast_interval** | **number** |  | [optional] [default to undefined]
**initial_cooldown** | **number** |  | [optional] [default to undefined]
**global_cooldown** | **number** |  | [optional] [default to undefined]
**ignore_prison_glyph** | **boolean** |  | [optional] [default to undefined]
**spell_breed** | **number** |  | [optional] [default to undefined]
**effects** | [**Array&lt;SpellEffect&gt;**](SpellEffect.md) |  | [optional] [default to undefined]
**critical_effects** | [**Array&lt;SpellEffect&gt;**](SpellEffect.md) |  | [optional] [default to undefined]

## Example

```typescript
import { SpellLevel } from 'dofusdude-ts';

const instance: SpellLevel = {
    ankama_id,
    grade,
    ap_cost,
    min_range,
    max_range,
    max_cast_per_turn,
    max_cast_per_target,
    max_global_cast_per_turn,
    max_global_cast_per_target,
    min_cast_interval,
    initial_cooldown,
    global_cooldown,
    ignore_prison_glyph,
    spell_breed,
    effects,
    critical_effects,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
