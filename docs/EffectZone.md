# EffectZone

Combat-cell area for this effect or activation context, not a geographic world area. Shape, size and inner size describe geometry. Actual affected cells can depend on position, direction and fight state. Each spell effect can have a different zone.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**raw** | **string** | Original compact zone encoding when the source provides one. | [optional] [default to undefined]
**shape** | [**ZoneShape**](ZoneShape.md) |  | [default to undefined]
**size** | **number** | Effective outer size of the area. A point has size 0. Whole-map and custom-cell shapes omit it. | [optional] [default to undefined]
**min_size** | **number** | Effective inner size for hollow or minimum-size shapes. Omitted when the shape has no inner boundary. | [optional] [default to undefined]
**cell_ids** | **Array&lt;number&gt;** | Explicit cells for a custom-cell shape. An empty array is normal for geometric shapes such as circles and does not mean the zone affects no cells. | [default to undefined]
**damage_decrease_step_percent** | **number** |  | [optional] [default to undefined]
**max_damage_decrease_apply_count** | **number** |  | [optional] [default to undefined]
**forced_direction** | **number** |  | [optional] [default to undefined]
**include_carried** | **boolean** |  | [optional] [default to undefined]
**stop_at_target** | **boolean** |  | [optional] [default to undefined]
**only_affect_in_sight_line** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { EffectZone } from 'dofusdude-ts';

const instance: EffectZone = {
    raw,
    shape,
    size,
    min_size,
    cell_ids,
    damage_decrease_step_percent,
    max_damage_decrease_apply_count,
    forced_direction,
    include_carried,
    stop_at_target,
    only_affect_in_sight_line,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
