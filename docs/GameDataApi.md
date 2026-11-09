# GameDataApi

All URIs are relative to *https://beta.api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAllAreas**](#getallareas) | **GET** /{game}/v1/{language}/areas/all | Get all areas|
|[**getAllClasses**](#getallclasses) | **GET** /{game}/v1/{language}/classes/all | Get all classes|
|[**getAllMonsters**](#getallmonsters) | **GET** /{game}/v1/{language}/monsters/all | Get all monsters|
|[**getAllSpells**](#getallspells) | **GET** /{game}/v1/{language}/spells/all | Get all spells|
|[**getAllSubareas**](#getallsubareas) | **GET** /{game}/v1/{language}/subareas/all | Get all subareas|
|[**getAllSuperAreas**](#getallsuperareas) | **GET** /{game}/v1/{language}/super-areas/all | Get all super-areas|
|[**getAreaById**](#getareabyid) | **GET** /{game}/v1/{language}/areas/{ankama_id} | Get one area|
|[**getAreas**](#getareas) | **GET** /{game}/v1/{language}/areas | List areas|
|[**getClassById**](#getclassbyid) | **GET** /{game}/v1/{language}/classes/{ankama_id} | Get one class|
|[**getClasses**](#getclasses) | **GET** /{game}/v1/{language}/classes | List classes|
|[**getMonsterById**](#getmonsterbyid) | **GET** /{game}/v1/{language}/monsters/{ankama_id} | Get one monster|
|[**getMonsters**](#getmonsters) | **GET** /{game}/v1/{language}/monsters | List monsters|
|[**getSpellById**](#getspellbyid) | **GET** /{game}/v1/{language}/spells/{ankama_id} | Get one spell|
|[**getSpells**](#getspells) | **GET** /{game}/v1/{language}/spells | List spells|
|[**getSubareaById**](#getsubareabyid) | **GET** /{game}/v1/{language}/subareas/{ankama_id} | Get one subarea|
|[**getSubareas**](#getsubareas) | **GET** /{game}/v1/{language}/subareas | List subareas|
|[**getSuperAreaById**](#getsuperareabyid) | **GET** /{game}/v1/{language}/super-areas/{ankama_id} | Get one super-area|
|[**getSuperAreas**](#getsuperareas) | **GET** /{game}/v1/{language}/super-areas | List super-areas|
|[**searchAreas**](#searchareas) | **GET** /{game}/v1/{language}/areas/search | Search areas|
|[**searchClasses**](#searchclasses) | **GET** /{game}/v1/{language}/classes/search | Search classes|
|[**searchMonsters**](#searchmonsters) | **GET** /{game}/v1/{language}/monsters/search | Search monsters|
|[**searchSpells**](#searchspells) | **GET** /{game}/v1/{language}/spells/search | Search spells|
|[**searchSubareas**](#searchsubareas) | **GET** /{game}/v1/{language}/subareas/search | Search subareas|
|[**searchSuperAreas**](#searchsuperareas) | **GET** /{game}/v1/{language}/super-areas/search | Search super-areas|

# **getAllAreas**
> MappedEntityCollection getAllAreas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)

const { status, data } = await apiInstance.getAllAreas(
    game,
    language
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Every complete localized area document. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllClasses**
> MappedEntityCollection getAllClasses()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)

const { status, data } = await apiInstance.getAllClasses(
    game,
    language
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Every complete localized class document. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllMonsters**
> MappedEntityCollection getAllMonsters()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let include: 'spells.grade' | 'spells'; //Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use `spells.grade` to embed the assigned spell grade. Use `spells` to embed every available grade of each assigned spell. (optional) (default to undefined)

const { status, data } = await apiInstance.getAllMonsters(
    game,
    language,
    include
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **include** | [**&#39;spells.grade&#39; | &#39;spells&#39;**]**Array<&#39;spells.grade&#39; &#124; &#39;spells&#39;>** | Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use &#x60;spells.grade&#x60; to embed the assigned spell grade. Use &#x60;spells&#x60; to embed every available grade of each assigned spell. | (optional) defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Every complete localized monster document. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllSpells**
> MappedEntityCollection getAllSpells()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)

const { status, data } = await apiInstance.getAllSpells(
    game,
    language
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Every complete localized spell document. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllSubareas**
> MappedEntityCollection getAllSubareas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)

const { status, data } = await apiInstance.getAllSubareas(
    game,
    language
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Every complete localized subarea document. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllSuperAreas**
> MappedEntityCollection getAllSuperAreas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)

const { status, data } = await apiInstance.getAllSuperAreas(
    game,
    language
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Every complete localized super-area document. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAreaById**
> WorldArea getAreaById()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let ankamaId: number; // (default to undefined)

const { status, data } = await apiInstance.getAreaById(
    game,
    language,
    ankamaId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **ankamaId** | [**number**] |  | defaults to undefined|


### Return type

**WorldArea**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Complete localized area document. |  -  |
|**404** | Entity not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAreas**
> MappedEntityCollection getAreas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let pageNumber: number; // (optional) (default to 1)
let pageSize: number; // (optional) (default to 20)
let fieldsAreas: 'all'; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAreas(
    game,
    language,
    pageNumber,
    pageSize,
    fieldsAreas
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **pageNumber** | [**number**] |  | (optional) defaults to 1|
| **pageSize** | [**number**] |  | (optional) defaults to 20|
| **fieldsAreas** | [**&#39;all&#39;**]**Array<&#39;all&#39;>** |  | (optional) defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Paginated areas. |  -  |
|**400** | Invalid pagination or field selection. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getClassById**
> Class getClassById()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let ankamaId: number; // (default to undefined)

const { status, data } = await apiInstance.getClassById(
    game,
    language,
    ankamaId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **ankamaId** | [**number**] |  | defaults to undefined|


### Return type

**Class**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Complete localized class document. |  -  |
|**404** | Entity not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getClasses**
> MappedEntityCollection getClasses()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let pageNumber: number; // (optional) (default to 1)
let pageSize: number; // (optional) (default to 20)
let fieldsClasses: 'all'; // (optional) (default to undefined)

const { status, data } = await apiInstance.getClasses(
    game,
    language,
    pageNumber,
    pageSize,
    fieldsClasses
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **pageNumber** | [**number**] |  | (optional) defaults to 1|
| **pageSize** | [**number**] |  | (optional) defaults to 20|
| **fieldsClasses** | [**&#39;all&#39;**]**Array<&#39;all&#39;>** |  | (optional) defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Paginated classes. |  -  |
|**400** | Invalid pagination or field selection. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMonsterById**
> Monster getMonsterById()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let ankamaId: number; // (default to undefined)
let include: 'spells.grade' | 'spells'; //Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use `spells.grade` to embed the assigned spell grade. Use `spells` to embed every available grade of each assigned spell. (optional) (default to undefined)

const { status, data } = await apiInstance.getMonsterById(
    game,
    language,
    ankamaId,
    include
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **ankamaId** | [**number**] |  | defaults to undefined|
| **include** | [**&#39;spells.grade&#39; | &#39;spells&#39;**]**Array<&#39;spells.grade&#39; &#124; &#39;spells&#39;>** | Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use &#x60;spells.grade&#x60; to embed the assigned spell grade. Use &#x60;spells&#x60; to embed every available grade of each assigned spell. | (optional) defaults to undefined|


### Return type

**Monster**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Complete localized monster document. |  -  |
|**404** | Entity not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMonsters**
> MappedEntityCollection getMonsters()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let pageNumber: number; // (optional) (default to 1)
let pageSize: number; // (optional) (default to 20)
let fieldsMonsters: 'all'; // (optional) (default to undefined)
let include: 'spells.grade' | 'spells'; //Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use `spells.grade` to embed the assigned spell grade. Use `spells` to embed every available grade of each assigned spell. (optional) (default to undefined)

const { status, data } = await apiInstance.getMonsters(
    game,
    language,
    pageNumber,
    pageSize,
    fieldsMonsters,
    include
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **pageNumber** | [**number**] |  | (optional) defaults to 1|
| **pageSize** | [**number**] |  | (optional) defaults to 20|
| **fieldsMonsters** | [**&#39;all&#39;**]**Array<&#39;all&#39;>** |  | (optional) defaults to undefined|
| **include** | [**&#39;spells.grade&#39; | &#39;spells&#39;**]**Array<&#39;spells.grade&#39; &#124; &#39;spells&#39;>** | Optional spell expansion for monster responses. Leave include unset to return spell URLs. Use &#x60;spells.grade&#x60; to embed the assigned spell grade. Use &#x60;spells&#x60; to embed every available grade of each assigned spell. | (optional) defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Paginated monsters. |  -  |
|**400** | Invalid pagination or field selection. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSpellById**
> Spell getSpellById()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let ankamaId: number; // (default to undefined)
let grade: number; //Select the spell variant identified by its explicit grade number, not its spell-level record ID or a player level. Returns the spell object with only that grade in levels. An unavailable grade returns 404. (optional) (default to undefined)

const { status, data } = await apiInstance.getSpellById(
    game,
    language,
    ankamaId,
    grade
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **ankamaId** | [**number**] |  | defaults to undefined|
| **grade** | [**number**] | Select the spell variant identified by its explicit grade number, not its spell-level record ID or a player level. Returns the spell object with only that grade in levels. An unavailable grade returns 404. | (optional) defaults to undefined|


### Return type

**Spell**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Complete localized spell document. |  -  |
|**404** | Entity not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSpells**
> MappedEntityCollection getSpells()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let pageNumber: number; // (optional) (default to 1)
let pageSize: number; // (optional) (default to 20)
let fieldsSpells: 'all'; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSpells(
    game,
    language,
    pageNumber,
    pageSize,
    fieldsSpells
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **pageNumber** | [**number**] |  | (optional) defaults to 1|
| **pageSize** | [**number**] |  | (optional) defaults to 20|
| **fieldsSpells** | [**&#39;all&#39;**]**Array<&#39;all&#39;>** |  | (optional) defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Paginated spells. |  -  |
|**400** | Invalid pagination or field selection. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSubareaById**
> WorldArea getSubareaById()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let ankamaId: number; // (default to undefined)

const { status, data } = await apiInstance.getSubareaById(
    game,
    language,
    ankamaId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **ankamaId** | [**number**] |  | defaults to undefined|


### Return type

**WorldArea**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Complete localized subarea document. |  -  |
|**404** | Entity not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSubareas**
> MappedEntityCollection getSubareas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let pageNumber: number; // (optional) (default to 1)
let pageSize: number; // (optional) (default to 20)
let fieldsSubareas: 'all'; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSubareas(
    game,
    language,
    pageNumber,
    pageSize,
    fieldsSubareas
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **pageNumber** | [**number**] |  | (optional) defaults to 1|
| **pageSize** | [**number**] |  | (optional) defaults to 20|
| **fieldsSubareas** | [**&#39;all&#39;**]**Array<&#39;all&#39;>** |  | (optional) defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Paginated subareas. |  -  |
|**400** | Invalid pagination or field selection. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSuperAreaById**
> WorldArea getSuperAreaById()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let ankamaId: number; // (default to undefined)

const { status, data } = await apiInstance.getSuperAreaById(
    game,
    language,
    ankamaId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **ankamaId** | [**number**] |  | defaults to undefined|


### Return type

**WorldArea**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Complete localized super-area document. |  -  |
|**404** | Entity not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSuperAreas**
> MappedEntityCollection getSuperAreas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let pageNumber: number; // (optional) (default to 1)
let pageSize: number; // (optional) (default to 20)
let fieldsSuperAreas: 'all'; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSuperAreas(
    game,
    language,
    pageNumber,
    pageSize,
    fieldsSuperAreas
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **pageNumber** | [**number**] |  | (optional) defaults to 1|
| **pageSize** | [**number**] |  | (optional) defaults to 20|
| **fieldsSuperAreas** | [**&#39;all&#39;**]**Array<&#39;all&#39;>** |  | (optional) defaults to undefined|


### Return type

**MappedEntityCollection**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Paginated super-areas. |  -  |
|**400** | Invalid pagination or field selection. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchAreas**
> Array<MappedEntityListEntry> searchAreas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let query: string; // (default to undefined)
let limit: number; // (optional) (default to 8)

const { status, data } = await apiInstance.searchAreas(
    game,
    language,
    query,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **query** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 8|


### Return type

**Array<MappedEntityListEntry>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Matching localized summaries. |  -  |
|**404** | No matching entities. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchClasses**
> Array<MappedEntityListEntry> searchClasses()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let query: string; // (default to undefined)
let limit: number; // (optional) (default to 8)

const { status, data } = await apiInstance.searchClasses(
    game,
    language,
    query,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **query** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 8|


### Return type

**Array<MappedEntityListEntry>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Matching localized summaries. |  -  |
|**404** | No matching entities. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchMonsters**
> Array<MappedEntityListEntry> searchMonsters()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let query: string; // (default to undefined)
let limit: number; // (optional) (default to 8)

const { status, data } = await apiInstance.searchMonsters(
    game,
    language,
    query,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **query** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 8|


### Return type

**Array<MappedEntityListEntry>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Matching localized summaries. |  -  |
|**404** | No matching entities. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchSpells**
> Array<MappedEntityListEntry> searchSpells()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let query: string; // (default to undefined)
let limit: number; // (optional) (default to 8)

const { status, data } = await apiInstance.searchSpells(
    game,
    language,
    query,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **query** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 8|


### Return type

**Array<MappedEntityListEntry>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Matching localized summaries. |  -  |
|**404** | No matching entities. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchSubareas**
> Array<MappedEntityListEntry> searchSubareas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let query: string; // (default to undefined)
let limit: number; // (optional) (default to 8)

const { status, data } = await apiInstance.searchSubareas(
    game,
    language,
    query,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **query** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 8|


### Return type

**Array<MappedEntityListEntry>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Matching localized summaries. |  -  |
|**404** | No matching entities. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchSuperAreas**
> Array<MappedEntityListEntry> searchSuperAreas()


### Example

```typescript
import {
    GameDataApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new GameDataApi(configuration);

let game: 'dofus3' | 'dofus3beta'; // (default to undefined)
let language: 'en' | 'fr' | 'de' | 'es' | 'pt'; // (default to undefined)
let query: string; // (default to undefined)
let limit: number; // (optional) (default to 8)

const { status, data } = await apiInstance.searchSuperAreas(
    game,
    language,
    query,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **game** | [**&#39;dofus3&#39; | &#39;dofus3beta&#39;**]**Array<&#39;dofus3&#39; &#124; &#39;dofus3beta&#39;>** |  | defaults to undefined|
| **language** | [**&#39;en&#39; | &#39;fr&#39; | &#39;de&#39; | &#39;es&#39; | &#39;pt&#39;**]**Array<&#39;en&#39; &#124; &#39;fr&#39; &#124; &#39;de&#39; &#124; &#39;es&#39; &#124; &#39;pt&#39;>** |  | defaults to undefined|
| **query** | [**string**] |  | defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to 8|


### Return type

**Array<MappedEntityListEntry>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Matching localized summaries. |  -  |
|**404** | No matching entities. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

