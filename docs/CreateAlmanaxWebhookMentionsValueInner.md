# CreateAlmanaxWebhookMentionsValueInner

Mention

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**discord_id** | **number** | User or role ID directly from Discord. Activate developer mode and right click a user or role to get them. | [optional] [default to undefined]
**is_role** | **boolean** | Whether an ID describes a role (true) or user (false). This is needed for formatting the mention command so Discord understands it. | [optional] [default to undefined]
**ping_days_before** | **number** | Get a mention days before the bonus comes up. It will post on the specified time. Also works when the interval is not daily. | [optional] [default to undefined]

## Example

```typescript
import { CreateAlmanaxWebhookMentionsValueInner } from 'dofusdude-ts';

const instance: CreateAlmanaxWebhookMentionsValueInner = {
    discord_id,
    is_role,
    ping_days_before,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
