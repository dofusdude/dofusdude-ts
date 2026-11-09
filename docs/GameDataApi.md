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

Returns every complete geographic area record, including its super-area reference and child subareas, without pagination. These relationships describe geography rather than combat effect zones.

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

Returns full playable-class definitions without pagination, including their assigned spells and each spell\'s available grades. Classes do not have monster grades. For smaller responses use the paginated classes endpoint or request one class by ID.

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

Returns complete monster definitions without pagination. Grades group each variant\'s statistics and spell assignments. Drop percentages are indexed by monster grade. Known spawn subareas are not live population or per-map spawn probabilities. Spell expansion is optional. This bulk response can be large, so prefer pagination when possible.

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

Returns complete spell definitions and all available grades without pagination. Each grade has its own costs, casting rules, normal effects and critical effects. Bulk responses can be large. Prefer pagination for interactive or incremental use.

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

Returns complete subareas, map membership and monster references without pagination. Maps belong to the subarea but are not guaranteed spawn locations for every associated monster. Prefer pagination for smaller responses.

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

Returns every complete super-area record and its child area references without pagination. A super-area groups geographic areas and supplies a world-map context. It is not a spell effect zone.

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

Returns an area\'s parent super-area and child subarea references. References contain an ID and localized name, not a complete nested record. Use the corresponding resource endpoint to load details. Matching numeric IDs in different resource types do not establish a relationship.

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

Lists geographic area summaries. An area belongs to a super-area and groups subareas. Request fields[areas]=all or an area detail record for those relationships. Use QUERY rather than GET for structured JSON filtering and sorting.

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

Returns a playable class, also called a breed in the client data. Its spells array contains full spell definitions. Each spell has its own levels array of spell grades. The class itself does not have grades, and a spell grade is not a character level.  Characteristic cost tiers describe point costs. Appearance bone and skin IDs are asset-renderer inputs, not image URLs. Use image_urls for ready-to-display artwork. IDs identify records independently of their translated names. Assigned spells can also be requested from the spells endpoint without loading the class again.

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

Lists playable classes, also called breeds in the client data. Results are compact summaries by default. Request fields[classes]=all for class characteristics, appearance and full assigned spell definitions. Spell grades belong to each spell, not to the class. Use the detail endpoint for one full class. Existing GET pagination and field parameters remain unchanged. Use QUERY for structured JSON filtering.

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

Returns a monster definition. race is its family and race.super_race is the broader monster grouping. Neither is a playable class. Each entry in grades is one monster variant with a grade number, a separate combat level, statistics and assigned spells. Select by explicit grade values, not array positions or a fixed assumed grade count.  Spell assignments belong to the enclosing monster grade. Their grade values identify spell variants and need not equal the monster grade. Default assignments contain URLs that already select the assigned spell grade. Follow them unchanged. include=spells.grade embeds just the assigned variant in each spell\'s levels array. include=spells embeds every available spell grade instead. These are optional expansions of an independently addressable resource.  Match drops[].rates_percent[].grade to the monster grade, not the spell grade. Percentages are base drop rates before player-specific modifiers. global_drops provides ranges instead of that grade-rate table. Client condition trees preserve and/or grouping but exclude server-only predicates. A missing tree does not guarantee eligibility, even when has_conditions is true.  spawn_locations identifies known spawn subareas and their geographic parents. subarea_maps lists subarea membership, not guaranteed spawn maps. preferred is a source preference flag, not a probability. The endpoint does not report live presence or per-map spawn percentages.

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

Lists monster summaries. Request fields[monsters]=all or the monster detail endpoint for variants, statistics, drop rates and known spawn subareas. A monster grade is a variant with its own combat level, not that level itself. Optional include values expand spell assignments. GET retains its existing pagination, field and include parameters. Use QUERY for structured filtering and sorting.

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

Returns a spell and its available grades in levels. A grade is a variant with its own action-point cost, range, casting limits and effects. Select by levels[].grade, not array position. levels[].ankama_id is the separate spell-level record ID. min_player_level records a player-level requirement and is not a grade number.  Pass grade to return only that variant inside the same spell object. An unavailable grade returns 404. For example, /spells/10198?grade=1 selects spell grade 1. This does not imply that monster grade 1 is the only monster variant using it.  Keep normal effects and critical_effects separate. Each effect has its own combat-cell zone, target_mask and triggers. These describe where, who and when it affects. Preview and script zones do not replace effect zones. Use resolved names and descriptions instead of decoding raw tokens. Templated text is localized display text, not a formula to parse. This endpoint supplies definitions, not a full fight simulation or final damage calculation.

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

Lists independent spell records as compact summaries. Request fields[spells]=all for their grades and effects, or use the spell detail endpoint for one spell. The levels field contains spell variants called grades, not player levels. Existing GET pagination and field parameters remain unchanged. Structured filters and sorting belong to QUERY and do not trim grades from matching spell records.

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

Returns one geographic subarea with its parent area and super-area, maps and monster references. Its level is a geographic difficulty indicator, not a monster grade or the combat level of every associated monster.  A map\'s ankama_id identifies the map. Interpret position_x and position_y with world_map_id because coordinates alone are not globally unique. Map membership does not prove that a monster spawns on every map or is currently present. Monster references can be followed through the monster endpoint for grade-specific statistics, base drop rates and known spawn subareas. This endpoint does not provide spawn percentages.

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

Lists subarea summaries. A subarea belongs to an area and super-area and contains maps. Request fields[subareas]=all or a detail record for map membership and monster associations. Associations are not live monster presence or per-map spawn probabilities.

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

Returns one broad geographic region with its child areas and world_map_id. Follow child area IDs to the areas endpoint to continue toward subareas and maps. World geography is independent of spell and weapon combat-cell geometry.

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

Lists summaries of the broadest geographic regions. The hierarchy is super-area to area to subarea to map. These world areas are unrelated to combat-cell effect zones. Request fields[super_areas]=all or a detail record for child area references and world-map context.

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

Searches localized geographic area names by relevance and returns compact summaries. Use the detail endpoint to obtain the parent super-area and child subareas.

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

Searches localized class names by relevance and returns compact summaries. Search is distinct from structured filtering. Use a returned ankama_id with the class detail endpoint for characteristics, appearance and assigned spell definitions.

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

Searches localized monster names by relevance and returns summaries. Each result identifies a monster definition, not one combat-level variant. Use the detail endpoint for grades, taxonomy, drops and known spawn subareas.

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

Searches localized spell names by relevance and returns compact summaries. The result ID identifies the spell, not a grade. Request the detail endpoint for available grades, or pass grade to that detail endpoint to select one variant.

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

Searches localized subarea names by relevance and returns summaries. Use the detail endpoint for parent areas, map positions and monster associations. Search results do not indicate live monster populations.

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

Searches localized super-area names by relevance. Results are geographic-region summaries. Use a returned ID with the detail endpoint for child areas and world-map context.

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

