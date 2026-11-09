# WorldMapReference

A map ID and its position within a world-map context. Maps can share coordinates in different contexts.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [optional] [default to undefined]
**position_x** | **number** |  | [optional] [default to undefined]
**position_y** | **number** |  | [optional] [default to undefined]
**world_map_id** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { WorldMapReference } from 'dofusdude-ts';

const instance: WorldMapReference = {
    ankama_id,
    position_x,
    position_y,
    world_map_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
