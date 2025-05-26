# MountsApi

All URIs are relative to *https://api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAllMountsList**](#getallmountslist) | **GET** /{game}/v1/{language}/mounts/all | List All Mounts|
|[**getMountsList**](#getmountslist) | **GET** /{game}/v1/{language}/mounts | List Mounts|
|[**getMountsSearch**](#getmountssearch) | **GET** /{game}/v1/{language}/mounts/search | Search Mounts|
|[**getMountsSingle**](#getmountssingle) | **GET** /{game}/v1/{language}/mounts/{ankama_id} | Single Mounts|

# **getAllMountsList**
> ListMounts getAllMountsList()

Retrieve all mounts with one request. This endpoint is just an alias for the a list with disabled pagination (page[size]=-1) and all fields[type] set.  If you want everything unfiltered, delete the other query parameters.  Be careful with testing or (god forbid) using /all in your browser, the returned json is huge and will slow down the browser!  Tip: set the HTTP Header \'Accept-Encoding: gzip\' for saving bandwidth. You will need to uncompress it on your end. Example with cURL: ``` curl -sH \'Accept-Encoding: gzip\' <api-endpoint> | gunzip - ```

### Example

```typescript
import {
    MountsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MountsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let filterFamilyName: string; //only results with the translated family name (optional) (default to undefined)
let acceptEncoding: 'gzip'; //optional compression for saving bandwidth (optional) (default to undefined)
let filterFamilyId: number; //only results with the unique family id (optional) (default to undefined)

const { status, data } = await apiInstance.getAllMountsList(
    language,
    game,
    filterFamilyName,
    acceptEncoding,
    filterFamilyId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **filterFamilyName** | [**string**] | only results with the translated family name | (optional) defaults to undefined|
| **acceptEncoding** | [**&#39;gzip&#39;**]**Array<&#39;gzip&#39;>** | optional compression for saving bandwidth | (optional) defaults to undefined|
| **filterFamilyId** | [**number**] | only results with the unique family id | (optional) defaults to undefined|


### Return type

**ListMounts**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** |  |  -  |
|**404** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMountsList**
> ListMounts getMountsList()

Retrieve a list of mounts.

### Example

```typescript
import {
    MountsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MountsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let filterFamilyName: string; //only results with the translated family name (optional) (default to undefined)
let pageSize: number; //size of the results from the list. -1 disables pagination and gets all in one response. (optional) (default to undefined)
let pageNumber: number; //page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. (optional) (default to undefined)
let fieldsMount: Set<'effects'>; //adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. (optional) (default to undefined)
let filterFamilyId: number; //only results with the unique family id (optional) (default to undefined)

const { status, data } = await apiInstance.getMountsList(
    language,
    game,
    filterFamilyName,
    pageSize,
    pageNumber,
    fieldsMount,
    filterFamilyId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **filterFamilyName** | [**string**] | only results with the translated family name | (optional) defaults to undefined|
| **pageSize** | [**number**] | size of the results from the list. -1 disables pagination and gets all in one response. | (optional) defaults to undefined|
| **pageNumber** | [**number**] | page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. | (optional) defaults to undefined|
| **fieldsMount** | **Array<&#39;effects&#39;>** | adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. | (optional) defaults to undefined|
| **filterFamilyId** | [**number**] | only results with the unique family id | (optional) defaults to undefined|


### Return type

**ListMounts**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** |  |  -  |
|**404** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMountsSearch**
> Array<Mount> getMountsSearch()

Search in all names and descriptions of mounts with a query.

### Example

```typescript
import {
    MountsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MountsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let query: string; //case sensitive search query (default to undefined)
let filterFamilyName: string; //only results with the translated family name (optional) (default to undefined)
let limit: number; //maximum number of returned results (optional) (default to 8)
let filterFamilyId: number; //only results with the unique family id (optional) (default to undefined)

const { status, data } = await apiInstance.getMountsSearch(
    language,
    game,
    query,
    filterFamilyName,
    limit,
    filterFamilyId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **query** | [**string**] | case sensitive search query | defaults to undefined|
| **filterFamilyName** | [**string**] | only results with the translated family name | (optional) defaults to undefined|
| **limit** | [**number**] | maximum number of returned results | (optional) defaults to 8|
| **filterFamilyId** | [**number**] | only results with the unique family id | (optional) defaults to undefined|


### Return type

**Array<Mount>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** |  |  -  |
|**404** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMountsSingle**
> Mount getMountsSingle()

Retrieve a specific mount with id.

### Example

```typescript
import {
    MountsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new MountsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let ankamaId: number; //identifier (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)

const { status, data } = await apiInstance.getMountsSingle(
    language,
    ankamaId,
    game
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **ankamaId** | [**number**] | identifier | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|


### Return type

**Mount**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |
|**400** |  |  -  |
|**404** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

