# ModelError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **number** | HTTP status code | [optional] [default to undefined]
**error** | **string** | HTTP status as text | [optional] [default to undefined]
**code** | **string** | API specific error identifier for switch-case handling | [optional] [default to undefined]
**message** | **string** | General, human-friendly error description | [optional] [default to undefined]
**details** | **string** | Detailed, human-friendly problem description adopting specific inputs of the request | [optional] [default to undefined]

## Example

```typescript
import { ModelError } from 'dofusdude-ts';

const instance: ModelError = {
    status,
    error,
    code,
    message,
    details,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
