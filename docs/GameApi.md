# GameApi

All URIs are relative to *https://api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getGameSearch**](#getgamesearch) | **GET** /{game}/v1/{language}/search | Game Search|
|[**getItemsAllSearch**](#getitemsallsearch) | **GET** /{game}/v1/{language}/items/search | Search All Items|

# **getGameSearch**
> Array<GameSearch> getGameSearch()

Search in all names and descriptions of all supported types in the game. For the list of supported types see the endpoint /dofus3/meta/search/types.

### Example

```typescript
import {
    GameApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let query: string; //search query (default to undefined)
let filterSearchIndex: Set<'items-consumables' | 'items-cosmetics' | 'items-resources' | 'items-equipment' | 'items-quest_items' | 'mounts' | 'sets'>; //only results with all specific type (optional) (default to undefined)
let limit: number; //maximum number of returned results (optional) (default to 8)
let fieldsItem: Set<'level' | 'image_urls' | 'type'>; //adds fields from the item search to the list entries if the hit is an item. Multiple comma separated values allowed. (optional) (default to undefined)
let filterTypeNameId: Set<string>; //multi-filter results with the english item type name, including \"mount\" and \"set\" from filter[search_index]. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". (optional) (default to undefined)

const { status, data } = await apiInstance.getGameSearch(
    language,
    game,
    query,
    filterSearchIndex,
    limit,
    fieldsItem,
    filterTypeNameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** | a valid language code | defaults to undefined|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** | game main \&#39;dofus3\&#39; or beta channel \&#39;dofus3beta\&#39; | defaults to undefined|
| **query** | [**string**] | search query | defaults to undefined|
| **filterSearchIndex** | **Array<&#39;items-consumables&#39; &#124; &#39;items-cosmetics&#39; &#124; &#39;items-resources&#39; &#124; &#39;items-equipment&#39; &#124; &#39;items-quest_items&#39; &#124; &#39;mounts&#39; &#124; &#39;sets&#39;>** | only results with all specific type | (optional) defaults to undefined|
| **limit** | [**number**] | maximum number of returned results | (optional) defaults to 8|
| **fieldsItem** | **Array<&#39;level&#39; &#124; &#39;image_urls&#39; &#124; &#39;type&#39;>** | adds fields from the item search to the list entries if the hit is an item. Multiple comma separated values allowed. | (optional) defaults to undefined|
| **filterTypeNameId** | **Set&lt;string&gt;** | multi-filter results with the english item type name, including \&quot;mount\&quot; and \&quot;set\&quot; from filter[search_index]. Add with \&quot;wood\&quot; or \&quot;+wood\&quot; and exclude with \&quot;-wood\&quot;. | (optional) defaults to undefined|


### Return type

**Array<GameSearch>**

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

# **getItemsAllSearch**
> Array<ListItemGeneral> getItemsAllSearch()

Search in all names and descriptions of Dofus items (including all subtypes) with a query.

### Example

```typescript
import {
    GameApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameApi(configuration);

let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; //a valid language code (default to undefined)
let game: 'dofus3' | 'dofus3beta'; //game main \'dofus3\' or beta channel \'dofus3beta\' (default to undefined)
let query: string; //case sensitive search query (default to undefined)
let filterMinLevel: number; //only results which level is equal or above this value (optional) (default to undefined)
let filterMaxLevel: number; //only results which level is equal or below this value (optional) (default to undefined)
let limit: number; //maximum number of returned results (optional) (default to 8)
let filterTypeNameId: Set<string>; //multi-filter results with the english type name. Add with \"wood\" or \"+wood\" and exclude with \"-wood\". (optional) (default to undefined)

const { status, data } = await apiInstance.getItemsAllSearch(
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

**Array<ListItemGeneral>**

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

