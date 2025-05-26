# QuestItemsApi

All URIs are relative to *https://api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAllItemsQuestList**](#getallitemsquestlist) | **GET** /{game}/v1/{language}/items/quest/all | List All Quest Items|
|[**getItemQuestSingle**](#getitemquestsingle) | **GET** /{game}/v1/{language}/items/quest/{ankama_id} | Single Quest Items|
|[**getItemsQuestList**](#getitemsquestlist) | **GET** /{game}/v1/{language}/items/quest | List Quest Items|
|[**getItemsQuestSearch**](#getitemsquestsearch) | **GET** /{game}/v1/{language}/items/quest/search | Search Quest Items|

# **getAllItemsQuestList**
> ListItems getAllItemsQuestList()

Retrieve all quest items with one request. This endpoint is just an alias for the a list with disabled pagination (page[size]=-1) and all fields[type] set.  If you want everything unfiltered, delete the other query parameters.  Be careful with testing or (god forbid) using /all in your browser, the returned json is huge and will slow down the browser!  Tip: set the HTTP Header \'Accept-Encoding: gzip\' for saving bandwidth. You will need to uncompress it on your end. Example with cURL: ``` curl -sH \'Accept-Encoding: gzip\' <api-endpoint> | gunzip - ```

### Example

```typescript
import {
    QuestItemsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new QuestItemsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let sortLevel: 'asc' | 'desc'; //sort the resulting list by level, default unsorted (optional) (default to undefined)
let filterMinLevel: number; //only results which level is equal or above this value (optional) (default to undefined)
let filterMaxLevel: number; //only results which level is equal or below this value (optional) (default to undefined)
let acceptEncoding: 'gzip'; //optional compression for saving bandwidth (optional) (default to undefined)
let filterTypeNameId: Set<string>; //multi-filter results with the english type name. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". (optional) (default to undefined)

const { status, data } = await apiInstance.getAllItemsQuestList(
    language,
    game,
    sortLevel,
    filterMinLevel,
    filterMaxLevel,
    acceptEncoding,
    filterTypeNameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **sortLevel** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** | sort the resulting list by level, default unsorted | (optional) defaults to undefined|
| **filterMinLevel** | [**number**] | only results which level is equal or above this value | (optional) defaults to undefined|
| **filterMaxLevel** | [**number**] | only results which level is equal or below this value | (optional) defaults to undefined|
| **acceptEncoding** | [**&#39;gzip&#39;**]**Array<&#39;gzip&#39;>** | optional compression for saving bandwidth | (optional) defaults to undefined|
| **filterTypeNameId** | **Set&lt;string&gt;** | multi-filter results with the english type name. Add with \&quot;wood\&quot; or \&quot;+wood\&quot; and exclude with \&quot;-wood\&quot;. | (optional) defaults to undefined|


### Return type

**ListItems**

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

# **getItemQuestSingle**
> Resource getItemQuestSingle()

Retrieve a specific quest item with id.

### Example

```typescript
import {
    QuestItemsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new QuestItemsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let ankamaId: number; //identifier (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)

const { status, data } = await apiInstance.getItemQuestSingle(
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

**Resource**

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

# **getItemsQuestList**
> ListItems getItemsQuestList()

Retrieve a list of quest items.

### Example

```typescript
import {
    QuestItemsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new QuestItemsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let sortLevel: 'asc' | 'desc'; //sort the resulting list by level, default unsorted (optional) (default to undefined)
let filterMinLevel: number; //only results which level is equal or above this value (optional) (default to undefined)
let filterMaxLevel: number; //only results which level is equal or below this value (optional) (default to undefined)
let pageSize: number; //size of the results from the list. -1 disables pagination and gets all in one response. (optional) (default to undefined)
let pageNumber: number; //page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. (optional) (default to undefined)
let fieldsItem: Set<'recipe' | 'description' | 'conditions' | 'effects'>; //adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. (optional) (default to undefined)
let filterTypeNameId: Set<string>; //multi-filter results with the english type name. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". (optional) (default to undefined)

const { status, data } = await apiInstance.getItemsQuestList(
    language,
    game,
    sortLevel,
    filterMinLevel,
    filterMaxLevel,
    pageSize,
    pageNumber,
    fieldsItem,
    filterTypeNameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **sortLevel** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** | sort the resulting list by level, default unsorted | (optional) defaults to undefined|
| **filterMinLevel** | [**number**] | only results which level is equal or above this value | (optional) defaults to undefined|
| **filterMaxLevel** | [**number**] | only results which level is equal or below this value | (optional) defaults to undefined|
| **pageSize** | [**number**] | size of the results from the list. -1 disables pagination and gets all in one response. | (optional) defaults to undefined|
| **pageNumber** | [**number**] | page number based on the current page[size]. So you could get page 1 with 8 entrys and page 2 would have entries 8 to 16. | (optional) defaults to undefined|
| **fieldsItem** | **Array<&#39;recipe&#39; &#124; &#39;description&#39; &#124; &#39;conditions&#39; &#124; &#39;effects&#39;>** | adds fields from their detail endpoint to the item list entries. Multiple comma separated values allowed. | (optional) defaults to undefined|
| **filterTypeNameId** | **Set&lt;string&gt;** | multi-filter results with the english type name. Add with \&quot;wood\&quot; or \&quot;+wood\&quot; and exclude with \&quot;-wood\&quot;. | (optional) defaults to undefined|


### Return type

**ListItems**

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

# **getItemsQuestSearch**
> Array<ListItem> getItemsQuestSearch()

Search in all names and descriptions of quest items with a query.

### Example

```typescript
import {
    QuestItemsApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new QuestItemsApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let query: string; //case sensitive search query (default to undefined)
let filterMinLevel: number; //only results which level is equal or above this value (optional) (default to undefined)
let filterMaxLevel: number; //only results which level is equal or below this value (optional) (default to undefined)
let limit: number; //maximum number of returned results (optional) (default to 8)
let filterTypeNameId: Set<string>; //multi-filter results with the english type name. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". (optional) (default to undefined)

const { status, data } = await apiInstance.getItemsQuestSearch(
    language,
    game,
    query,
    filterMinLevel,
    filterMaxLevel,
    limit,
    filterTypeNameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **query** | [**string**] | case sensitive search query | defaults to undefined|
| **filterMinLevel** | [**number**] | only results which level is equal or above this value | (optional) defaults to undefined|
| **filterMaxLevel** | [**number**] | only results which level is equal or below this value | (optional) defaults to undefined|
| **limit** | [**number**] | maximum number of returned results | (optional) defaults to 8|
| **filterTypeNameId** | **Set&lt;string&gt;** | multi-filter results with the english type name. Add with \&quot;wood\&quot; or \&quot;+wood\&quot; and exclude with \&quot;-wood\&quot;. | (optional) defaults to undefined|


### Return type

**Array<ListItem>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Quest Items Found |  -  |
|**400** |  |  -  |
|**404** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

