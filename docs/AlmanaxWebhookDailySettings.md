# AlmanaxWebhookDailySettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timezone** | **string** | Timezone of your community to determine midnight. | [optional] [default to 'Europe/Paris']
**midnight_offset** | **number** | Hours added to midnight at the selected timezone. 8 &#x3D; 8:00 in the morning. | [optional] [default to 0]

## Example

```typescript
import { AlmanaxWebhookDailySettings } from 'dofusdude-ts';

const instance: AlmanaxWebhookDailySettings = {
    timezone,
    midnight_offset,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
