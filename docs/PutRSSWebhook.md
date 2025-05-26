# PutRSSWebhook



## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**whitelist** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**blacklist** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**subscriptions** | **Set&lt;string&gt;** | Get the available subscriptions with /meta/webhooks/rss | [optional] [default to undefined]
**preview_length** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { PutRSSWebhook } from 'dofusdude-ts';

const instance: PutRSSWebhook = {
    whitelist,
    blacklist,
    subscriptions,
    preview_length,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
