# WeaponCombat

Weapon attack targeting and area geometry. Available for weapon equipment. This is separate from spell effect zones.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**zone** | [**EffectZone**](EffectZone.md) |  | [default to undefined]
**cast_in_line** | **boolean** |  | [default to undefined]
**cast_in_diagonal** | **boolean** |  | [default to undefined]
**requires_line_of_sight** | **boolean** |  | [default to undefined]

## Example

```typescript
import { WeaponCombat } from 'dofusdude-ts';

const instance: WeaponCombat = {
    zone,
    cast_in_line,
    cast_in_diagonal,
    requires_line_of_sight,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
