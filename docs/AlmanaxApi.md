# AlmanaxApi

All URIs are relative to *https://api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAlmanaxDate**](#getalmanaxdate) | **GET** /dofus3/v1/{language}/almanax/{date} | Single Almanax Date|
|[**getAlmanaxRange**](#getalmanaxrange) | **GET** /dofus3/v1/{language}/almanax | Almanax Range|

# **getAlmanaxDate**
> Almanax getAlmanaxDate()

Get a single date. There are not more details in the returned object than the normal range endpoint.

### Example

```typescript
import {
    AlmanaxApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new AlmanaxApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //code (default to undefined)
let date: string; //yyyy-mm-dd (default to undefined)
let level: number; //character level for the reward_xp field (optional) (default to undefined)

const { status, data } = await apiInstance.getAlmanaxDate(
    language,
    date,
    level
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | code | defaults to undefined|
| **date** | [**string**] | yyyy-mm-dd | defaults to undefined|
| **level** | [**number**] | character level for the reward_xp field | (optional) defaults to undefined|


### Return type

**Almanax**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAlmanaxRange**
> Array<Almanax> getAlmanaxRange()

Get a range of dates, defaults to today + 6 following days but can specified by the query parameters.   filter[bonus_type] can be used seperately and does not have an effect on the other parameters.  range[from] changes the start date, everything else defaults to 6 following dates from this start date.  range[to] when used without anything else, it will use today as start date and this parameter as end. All ranges are inclusive.  range[from] + range[to] = inclusive range over the specified dates, should never be farther apart than 35 days.  range[from|to] + range[size] no need to specify the date, just following days with [from] (0 is today) or go backwards in time with only [to] and [size].  Not all combinations are listed but this should give you an idea how to they could work.

### Example

```typescript
import {
    AlmanaxApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new AlmanaxApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //code (default to undefined)
let filterBonusType: string; //ids from meta/{language}/almanax/bonuses (optional) (default to undefined)
let rangeFrom: string; //yyyy-mm-dd (optional) (default to undefined)
let rangeTo: string; //yyyy-mm-dd (optional) (default to undefined)
let rangeSize: number; //Size of the returned range. Disable to fully use the range by setting size to -1. (optional) (default to undefined)
let timezone: string; //determine what the current time is. If you live in Brazil, \"today\" will be hours apart from Paris. Use your timezone to get results relative to your location. (optional) (default to 'Europe/Paris')
let level: number; //character level for the reward_xp field (optional) (default to undefined)

const { status, data } = await apiInstance.getAlmanaxRange(
    language,
    filterBonusType,
    rangeFrom,
    rangeTo,
    rangeSize,
    timezone,
    level
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | code | defaults to undefined|
| **filterBonusType** | [**string**] | ids from meta/{language}/almanax/bonuses | (optional) defaults to undefined|
| **rangeFrom** | [**string**] | yyyy-mm-dd | (optional) defaults to undefined|
| **rangeTo** | [**string**] | yyyy-mm-dd | (optional) defaults to undefined|
| **rangeSize** | [**number**] | Size of the returned range. Disable to fully use the range by setting size to -1. | (optional) defaults to undefined|
| **timezone** | [**string**] | determine what the current time is. If you live in Brazil, \&quot;today\&quot; will be hours apart from Paris. Use your timezone to get results relative to your location. | (optional) defaults to 'Europe/Paris'|
| **level** | [**number**] | character level for the reward_xp field | (optional) defaults to undefined|


### Return type

**Array<Almanax>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

