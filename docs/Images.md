# Images

All images except icon are rendered in the background which can take some time (up to hours if all data is completely generated from scratch). Because of this, they can be null if they are not yet rendered.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**icon** | **string** | 64x64 px, always available | [optional] [default to undefined]
**sd** | **string** | around 2x the resolution of icon | [optional] [default to undefined]
**hq** | **string** | around 2x the resolution of sd | [optional] [default to undefined]
**hd** | **string** | around 2x the resolution of hd | [optional] [default to undefined]

## Example

```typescript
import { Images } from 'dofusdude-ts';

const instance: Images = {
    icon,
    sd,
    hq,
    hd,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
