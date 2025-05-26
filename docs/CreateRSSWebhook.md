# CreateRSSWebhook



## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**whitelist** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**blacklist** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**subscriptions** | **Set&lt;string&gt;** | Get the available subscriptions with /meta/webhooks/rss | [default to undefined]
**format** | **string** |  | [default to undefined]
**preview_length** | **number** |  | [optional] [default to undefined]
**callback** | **string** | Discord Webhook URL | [default to undefined]

## Example

```typescript
import { CreateRSSWebhook } from 'dofusdude-ts';

const instance: CreateRSSWebhook = {
    whitelist,
    blacklist,
    subscriptions,
    format,
    preview_length,
    callback,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
