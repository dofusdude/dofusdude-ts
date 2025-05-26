# PutAlmanaxWebhook


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bonus_whitelist** | **Array&lt;string&gt;** | from all available bonuses (ids) from /dofus3/meta/{language}/almanax/bonuses. Delete old entries with empty array []. Just null changes nothing. | [optional] [default to undefined]
**bonus_blacklist** | **Array&lt;string&gt;** | from all available bonuses (ids) from /dofus3/meta/{language}/almanax/bonuses. Delete old entries with empty array []. Just null changes nothing. | [optional] [default to undefined]
**subscriptions** | **Array&lt;string&gt;** | Get the available subscriptions with /meta/webhooks/almanax | [optional] [default to undefined]
**daily_settings** | [**CreateAlmanaxWebhookDailySettings**](CreateAlmanaxWebhookDailySettings.md) |  | [optional] [default to undefined]
**iso_date** | **boolean** | If false, it will use common local time formats and weekday translations. If true, the format is YYYY-MM-DD. | [optional] [default to false]
**mentions** | **{ [key: string]: Array&lt;CreateAlmanaxWebhookMentionsValueInner&gt;; }** | Almanax bonus ids mapped to array of mentions. | [optional] [default to undefined]
**intervals** | **Set&lt;string&gt;** |  | [optional] [default to undefined]
**weekly_weekday** | **string** | When to post the weekly preview at the specified time. | [optional] [default to undefined]

## Example

```typescript
import { PutAlmanaxWebhook } from 'dofusdude-ts';

const instance: PutAlmanaxWebhook = {
    bonus_whitelist,
    bonus_blacklist,
    subscriptions,
    daily_settings,
    iso_date,
    mentions,
    intervals,
    weekly_weekday,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
