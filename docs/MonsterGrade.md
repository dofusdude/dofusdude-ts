# MonsterGrade


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**grade** | **number** |  | [default to undefined]
**level** | **number** |  | [default to undefined]
**life_points** | **number** |  | [optional] [default to undefined]
**action_points** | **number** |  | [optional] [default to undefined]
**movement_points** | **number** |  | [optional] [default to undefined]
**grade_xp** | **number** |  | [optional] [default to undefined]
**neutral_resistance** | **number** |  | [optional] [default to undefined]
**earth_resistance** | **number** |  | [optional] [default to undefined]
**fire_resistance** | **number** |  | [optional] [default to undefined]
**water_resistance** | **number** |  | [optional] [default to undefined]
**air_resistance** | **number** |  | [optional] [default to undefined]
**pa_dodge** | **number** |  | [optional] [default to undefined]
**pm_dodge** | **number** |  | [optional] [default to undefined]
**damage_bonus** | **number** |  | [optional] [default to undefined]
**percent_damage_bonus** | **number** |  | [optional] [default to undefined]
**critical_hit_bonus** | **number** |  | [optional] [default to undefined]
**initiative_bonus** | **number** |  | [optional] [default to undefined]
**tackle_bonus** | **number** |  | [optional] [default to undefined]
**tackle_evade** | **number** |  | [optional] [default to undefined]
**max_summon** | **number** |  | [optional] [default to undefined]
**bonus_characteristics** | **{ [key: string]: number; }** |  | [optional] [default to undefined]
**spells** | [**Array&lt;MonsterGradeSpellsInner&gt;**](MonsterGradeSpellsInner.md) | Spells assigned to this exact monster grade. | [default to undefined]

## Example

```typescript
import { MonsterGrade } from 'dofusdude-ts';

const instance: MonsterGrade = {
    grade,
    level,
    life_points,
    action_points,
    movement_points,
    grade_xp,
    neutral_resistance,
    earth_resistance,
    fire_resistance,
    water_resistance,
    air_resistance,
    pa_dodge,
    pm_dodge,
    damage_bonus,
    percent_damage_bonus,
    critical_hit_bonus,
    initiative_bonus,
    tackle_bonus,
    tackle_evade,
    max_summon,
    bonus_characteristics,
    spells,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
