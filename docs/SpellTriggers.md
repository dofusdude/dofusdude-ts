# SpellTriggers

Determines when an effect activates. Events are not additional effects to apply unconditionally. Use logic with the resolved event names and descriptions instead of parsing raw tokens.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**raw** | **string** | Original trigger tokens retained for lossless debugging. | [default to undefined]
**logic** | **string** |  | [optional] [default to undefined]
**events** | [**Array&lt;SpellTrigger&gt;**](SpellTrigger.md) |  | [default to undefined]

## Example

```typescript
import { SpellTriggers } from 'dofusdude-ts';

const instance: SpellTriggers = {
    raw,
    logic,
    events,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
