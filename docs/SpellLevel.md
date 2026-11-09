# SpellLevel

One grade of a spell. The levels array contains these spell variants, not player levels. Grade numbers are local to the containing spell and are independent of monster grades.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** | ID of the spell-level definition. Different from the parent spell ID and from the grade number. Used by explicit spell-level references such as script spell_level_ids. | [optional] [default to undefined]
**grade** | **number** | Number identifying this variant within its spell. Select by this value, not by the array position. Used by the spell detail endpoint\&#39;s grade parameter. | [optional] [default to undefined]
**ap_cost** | **number** | Action points required to cast this spell grade. | [optional] [default to undefined]
**critical_hit_probability** | **number** | Base critical-hit percentage recorded for this spell grade, before fighter-specific modifiers. | [optional] [default to undefined]
**min_player_level** | **number** | Player-level requirement recorded for this spell grade. This is not its grade number or a monster combat level. | [optional] [default to undefined]
**min_range** | **number** | Minimum casting range in combat cells. | [optional] [default to undefined]
**max_range** | **number** | Maximum casting range in combat cells as defined by this grade. | [optional] [default to undefined]
**max_cast_per_turn** | **number** | Per-caster cast limit within a turn as recorded by the source. | [optional] [default to undefined]
**max_cast_per_target** | **number** |  | [optional] [default to undefined]
**max_global_cast_per_turn** | **number** |  | [optional] [default to undefined]
**max_global_cast_per_target** | **number** |  | [optional] [default to undefined]
**min_cast_interval** | **number** | Minimum interval between casts, measured in fight turns. | [optional] [default to undefined]
**initial_cooldown** | **number** | Initial wait before casting, measured in fight turns. | [optional] [default to undefined]
**global_cooldown** | **number** |  | [optional] [default to undefined]
**ignore_prison_glyph** | **boolean** |  | [optional] [default to undefined]
**spell_breed** | **number** |  | [optional] [default to undefined]
**states_criterion** | [**EligibilityNode**](EligibilityNode.md) | Available client-side state requirements for this spell grade. Null does not assert that the server imposes no restriction. | [optional] [default to undefined]
**preview_zones** | [**Array&lt;SpellPreviewZone&gt;**](SpellPreviewZone.md) | Client preview and activation geometry for this grade. Use each effect\&#39;s zone for its actual effect-area definition. | [optional] [default to undefined]
**effects** | [**Array&lt;SpellEffect&gt;**](SpellEffect.md) | Normal-cast effects for this grade. Each entry has independent targeting and area geometry. | [optional] [default to undefined]
**critical_effects** | [**Array&lt;SpellEffect&gt;**](SpellEffect.md) | Critical-cast effects for this grade. Keep separate from normal effects rather than applying both arrays to every cast. | [optional] [default to undefined]

## Example

```typescript
import { SpellLevel } from 'dofusdude-ts';

const instance: SpellLevel = {
    ankama_id,
    grade,
    ap_cost,
    critical_hit_probability,
    min_player_level,
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
    states_criterion,
    preview_zones,
    effects,
    critical_effects,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
