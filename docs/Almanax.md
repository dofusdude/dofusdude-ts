# Almanax


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bonus** | [**AlmanaxBonus**](AlmanaxBonus.md) |  | [optional] [default to undefined]
**date** | **string** |  | [optional] [default to undefined]
**tribute** | [**AlmanaxTribute**](AlmanaxTribute.md) |  | [optional] [default to undefined]
**reward_kamas** | **number** | Amount of Kamas you get as reward for finishing this Almanax quest. | [optional] [default to undefined]
**reward_xp** | **number** | Optional field that shows when a level is given in the request. Shows the experience points you get this day for finishing this Almanax quest. | [optional] [default to undefined]

## Example

```typescript
import { Almanax } from 'dofusdude-ts';

const instance: Almanax = {
    bonus,
    date,
    tribute,
    reward_kamas,
    reward_xp,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
