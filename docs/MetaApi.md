# MetaApi

All URIs are relative to *https://api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getGameSearchTypes**](#getgamesearchtypes) | **GET** /{game}/v1/meta/search/types | Available Game Search Types|
|[**getItemTypes**](#getitemtypes) | **GET** /{game}/v1/meta/items/types | Available Item Types|
|[**getMetaAlmanaxBonuses**](#getmetaalmanaxbonuses) | **GET** /dofus3/v1/meta/{language}/almanax/bonuses | Available Almanax Bonuses|
|[**getMetaAlmanaxBonusesSearch**](#getmetaalmanaxbonusessearch) | **GET** /dofus3/v1/meta/{language}/almanax/bonuses/search | Search Available Almanax Bonuses|
|[**getMetaElements**](#getmetaelements) | **GET** /{game}/v1/meta/elements | Effects and Condition Elements|
|[**getMetaVersion**](#getmetaversion) | **GET** /{game}/v1/meta/version | Game Version|

# **getGameSearchTypes**
> Array<string> getGameSearchTypes()

Get all types for /{game}/v1/{lang}/search available for filtering. All names are english for comparing them inside applications. Order is fixed so you can compare indices instead of strings.

### Example

```typescript
import {
    MetaApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MetaApi(configuration);

let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)

const { status, data } = await apiInstance.getGameSearchTypes(
    game
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|


### Return type

**Array<string>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getItemTypes**
> Array<string> getItemTypes()

Get all types of all items. Primarily used for filtering more detailed types in listings or search endpoints. All names are english for comparing them inside applications. Ordering is not guaranteed to persist with game updates.

### Example

```typescript
import {
    MetaApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MetaApi(configuration);

let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)

const { status, data } = await apiInstance.getItemTypes(
    game
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|


### Return type

**Array<string>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMetaAlmanaxBonuses**
> Array<GetMetaAlmanaxBonuses200ResponseInner> getMetaAlmanaxBonuses()

Get all the available bonuses and their id for filtering them in the range endpoint.

### Example

```typescript
import {
    MetaApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MetaApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)

const { status, data } = await apiInstance.getMetaAlmanaxBonuses(
    language
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|


### Return type

**Array<GetMetaAlmanaxBonuses200ResponseInner>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMetaAlmanaxBonusesSearch**
> Array<GetMetaAlmanaxBonuses200ResponseInner> getMetaAlmanaxBonusesSearch()

Search all the available bonuses and their id for filtering them in the range endpoint.

### Example

```typescript
import {
    MetaApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MetaApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let query: string; //case sensitive search query (default to undefined)
let limit: number; //maximum number of returned results (optional) (default to undefined)

const { status, data } = await apiInstance.getMetaAlmanaxBonusesSearch(
    language,
    query,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **query** | [**string**] | case sensitive search query | defaults to undefined|
| **limit** | [**number**] | maximum number of returned results | (optional) defaults to undefined|


### Return type

**Array<GetMetaAlmanaxBonuses200ResponseInner>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMetaElements**
> Array<string> getMetaElements()

Get the mappings for all specific elements that are linked in the dataset. All names are english. Translations are not needed because of a global unique id which is the index inside the array. Future elements will get a higher id.

### Example

```typescript
import {
    MetaApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MetaApi(configuration);

let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)

const { status, data } = await apiInstance.getMetaElements(
    game
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|


### Return type

**Array<string>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMetaVersion**
> Version getMetaVersion()

The current game version of the hosted data.

### Example

```typescript
import {
    MetaApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MetaApi(configuration);

let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)

const { status, data } = await apiInstance.getMetaVersion(
    game
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|


### Return type

**Version**

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

