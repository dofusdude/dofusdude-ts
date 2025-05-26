# SetsApi

All URIs are relative to *https://api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAllSetsList**](#getallsetslist) | **GET** /{game}/v1/{language}/sets/all | List All Sets|
|[**getSetsList**](#getsetslist) | **GET** /{game}/v1/{language}/sets | List Sets|
|[**getSetsSearch**](#getsetssearch) | **GET** /{game}/v1/{language}/sets/search | Search Sets|
|[**getSetsSingle**](#getsetssingle) | **GET** /{game}/v1/{language}/sets/{ankama_id} | Single Sets|

# **getAllSetsList**
> ListEquipmentSets getAllSetsList()

Retrieve all sets with one request. This endpoint is just an alias for the a list with disabled pagination (page[size]=-1) and all fields[type] set.  If you want everything unfiltered, delete the other query parameters.  Be careful with testing or (god forbid) using /all in your browser, the returned json is huge and will slow down the browser!  Tip: set the HTTP Header \'Accept-Encoding: gzip\' for saving bandwidth. You will need to uncompress it on your end. Example with cURL: ``` curl -sH \'Accept-Encoding: gzip\' <api-endpoint> | gunzip - ```

### Example

```typescript
import {
    SetsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new SetsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let sortLevel: 'asc' | 'desc'; //sort the resulting list by level, default unsorted (optional) (default to undefined)
let filterMinHighestEquipmentLevel: number; //only results where the equipment with the highest level is above or equal to this value (optional) (default to undefined)
let filterMaxHighestEquipmentLevel: number; //only results where the equipment with the highest level is below or equal to this value (optional) (default to undefined)
let acceptEncoding: 'gzip'; //optional compression for saving bandwidth (optional) (default to undefined)
let filterContainsCosmeticsOnly: boolean; //filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. (optional) (default to undefined)
let filterContainsCosmetics: boolean; //filter sets based on if they got cosmetic items in it. (optional) (default to undefined)

const { status, data } = await apiInstance.getAllSetsList(
    language,
    game,
    sortLevel,
    filterMinHighestEquipmentLevel,
    filterMaxHighestEquipmentLevel,
    acceptEncoding,
    filterContainsCosmeticsOnly,
    filterContainsCosmetics
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **sortLevel** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** | sort the resulting list by level, default unsorted | (optional) defaults to undefined|
| **filterMinHighestEquipmentLevel** | [**number**] | only results where the equipment with the highest level is above or equal to this value | (optional) defaults to undefined|
| **filterMaxHighestEquipmentLevel** | [**number**] | only results where the equipment with the highest level is below or equal to this value | (optional) defaults to undefined|
| **acceptEncoding** | [**&#39;gzip&#39;**]**Array<&#39;gzip&#39;>** | optional compression for saving bandwidth | (optional) defaults to undefined|
| **filterContainsCosmeticsOnly** | [**boolean**] | filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. | (optional) defaults to undefined|
| **filterContainsCosmetics** | [**boolean**] | filter sets based on if they got cosmetic items in it. | (optional) defaults to undefined|


### Return type

**ListEquipmentSets**

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

# **getSetsList**
> ListEquipmentSets getSetsList()

Retrieve a list of sets.

### Example

```typescript
import {
    SetsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new SetsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let sortLevel: 'asc' | 'desc'; //sort the resulting list by level, default unsorted (optional) (default to undefined)
let filterMinHighestEquipmentLevel: number; //only results where the equipment with the highest level is above or equal to this value (optional) (default to undefined)
let filterMaxHighestEquipmentLevel: number; //only results where the equipment with the highest level is below or equal to this value (optional) (default to undefined)
let pageSize: number; //size of the results from the list. -1 disables pagination and gets all in one response. (optional) (default to undefined)
let pageNumber: number; //page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. (optional) (default to undefined)
let fieldsSet: Set<'effects' | 'equipment_ids'>; //adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. (optional) (default to undefined)
let filterContainsCosmeticsOnly: boolean; //filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. (optional) (default to undefined)
let filterContainsCosmetics: boolean; //filter sets based on if they got cosmetic items in it. (optional) (default to undefined)

const { status, data } = await apiInstance.getSetsList(
    language,
    game,
    sortLevel,
    filterMinHighestEquipmentLevel,
    filterMaxHighestEquipmentLevel,
    pageSize,
    pageNumber,
    fieldsSet,
    filterContainsCosmeticsOnly,
    filterContainsCosmetics
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **sortLevel** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** | sort the resulting list by level, default unsorted | (optional) defaults to undefined|
| **filterMinHighestEquipmentLevel** | [**number**] | only results where the equipment with the highest level is above or equal to this value | (optional) defaults to undefined|
| **filterMaxHighestEquipmentLevel** | [**number**] | only results where the equipment with the highest level is below or equal to this value | (optional) defaults to undefined|
| **pageSize** | [**number**] | size of the results from the list. -1 disables pagination and gets all in one response. | (optional) defaults to undefined|
| **pageNumber** | [**number**] | page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. | (optional) defaults to undefined|
| **fieldsSet** | **Array<&#39;effects&#39; &#124; &#39;equipment_ids&#39;>** | adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. | (optional) defaults to undefined|
| **filterContainsCosmeticsOnly** | [**boolean**] | filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. | (optional) defaults to undefined|
| **filterContainsCosmetics** | [**boolean**] | filter sets based on if they got cosmetic items in it. | (optional) defaults to undefined|


### Return type

**ListEquipmentSets**

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

# **getSetsSearch**
> Array<ListEquipmentSet> getSetsSearch()

Search in all names and descriptions of sets with a query.

### Example

```typescript
import {
    SetsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new SetsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let query: string; //case sensitive search query (default to undefined)
let filterMinHighestEquipmentLevel: number; //only results where the equipment with the highest level is above or equal to this value (optional) (default to undefined)
let filterMaxHighestEquipmentLevel: number; //only results where the equipment with the highest level is below or equal to this value (optional) (default to undefined)
let limit: number; //maximum number of returned results (optional) (default to 8)
let filterContainsCosmeticsOnly: boolean; //filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. (optional) (default to undefined)
let filterContainsCosmetics: boolean; //filter sets based on if they got any cosmetic items in it (optional) (default to undefined)

const { status, data } = await apiInstance.getSetsSearch(
    language,
    game,
    query,
    filterMinHighestEquipmentLevel,
    filterMaxHighestEquipmentLevel,
    limit,
    filterContainsCosmeticsOnly,
    filterContainsCosmetics
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **query** | [**string**] | case sensitive search query | defaults to undefined|
| **filterMinHighestEquipmentLevel** | [**number**] | only results where the equipment with the highest level is above or equal to this value | (optional) defaults to undefined|
| **filterMaxHighestEquipmentLevel** | [**number**] | only results where the equipment with the highest level is below or equal to this value | (optional) defaults to undefined|
| **limit** | [**number**] | maximum number of returned results | (optional) defaults to 8|
| **filterContainsCosmeticsOnly** | [**boolean**] | filter sets based on if they only got cosmetic items in it. If true, the item ids are for the cosmetic endpoints instead of equipment. | (optional) defaults to undefined|
| **filterContainsCosmetics** | [**boolean**] | filter sets based on if they got any cosmetic items in it | (optional) defaults to undefined|


### Return type

**Array<ListEquipmentSet>**

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

# **getSetsSingle**
> EquipmentSet getSetsSingle()

Retrieve a specific set with id.

### Example

```typescript
import {
    SetsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new SetsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let ankamaId: number; //identifier (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)

const { status, data } = await apiInstance.getSetsSingle(
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

**EquipmentSet**

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

