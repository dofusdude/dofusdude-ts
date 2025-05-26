# WebhooksApi

All URIs are relative to *https://api.dofusdu.de*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteWebhooksAlmanaxId**](#deletewebhooksalmanaxid) | **DELETE** /webhooks/almanax/{id} | Unregister Almanax Hook|
|[**deleteWebhooksRssId**](#deletewebhooksrssid) | **DELETE** /webhooks/rss/{id} | Unregister RSS Hook|
|[**deleteWebhooksTwitterId**](#deletewebhookstwitterid) | **DELETE** /webhooks/twitter/{id} | Unregister Twitter Hook|
|[**getMetaWebhooksAlmanax**](#getmetawebhooksalmanax) | **GET** /meta/webhooks/almanax | Get Almanax Hook Metainfo|
|[**getMetaWebhooksRss**](#getmetawebhooksrss) | **GET** /meta/webhooks/rss | Get RSS Hook Metainfo|
|[**getMetaWebhooksTwitter**](#getmetawebhookstwitter) | **GET** /meta/webhooks/twitter | Get Twitter Hook Metainfo|
|[**getWebhooksAlmanaxId**](#getwebhooksalmanaxid) | **GET** /webhooks/almanax/{id} | Get Almanax Hook|
|[**getWebhooksRssId**](#getwebhooksrssid) | **GET** /webhooks/rss/{id} | Get RSS Hook|
|[**getWebhooksTwitterId**](#getwebhookstwitterid) | **GET** /webhooks/twitter/{id} | Get Twitter Hook|
|[**postWebhooksAlmanax**](#postwebhooksalmanax) | **POST** /webhooks/almanax | Register Almanax Hook|
|[**postWebhooksRss**](#postwebhooksrss) | **POST** /webhooks/rss | Register RSS Hook|
|[**postWebhooksTwitter**](#postwebhookstwitter) | **POST** /webhooks/twitter | Register Twitter Hook|
|[**putWebhooksAlmanaxId**](#putwebhooksalmanaxid) | **PUT** /webhooks/almanax/{id} | Update Almanax Hook|
|[**putWebhooksRssId**](#putwebhooksrssid) | **PUT** /webhooks/rss/{id} | Update RSS Hook|
|[**putWebhooksTwitterId**](#putwebhookstwitterid) | **PUT** /webhooks/twitter/{id} | Update Twitter Hook|

# **deleteWebhooksAlmanaxId**
> deleteWebhooksAlmanaxId()

Delete a Webhook from the service.

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)

const { status, data } = await apiInstance.deleteWebhooksAlmanaxId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteWebhooksRssId**
> deleteWebhooksRssId()

Delete a Webhook from the service.

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)

const { status, data } = await apiInstance.deleteWebhooksRssId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteWebhooksTwitterId**
> deleteWebhooksTwitterId()

Delete a Webhook from the service.

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)

const { status, data } = await apiInstance.deleteWebhooksTwitterId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | No Content |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMetaWebhooksAlmanax**
> GetMetaWebhooksTwitter200Response getMetaWebhooksAlmanax()

Get a list of all available subscriptions. 

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

const { status, data } = await apiInstance.getMetaWebhooksAlmanax();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**GetMetaWebhooksTwitter200Response**

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

# **getMetaWebhooksRss**
> GetMetaWebhooksTwitter200Response getMetaWebhooksRss()

Get a list of all available subscriptions. 

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

const { status, data } = await apiInstance.getMetaWebhooksRss();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**GetMetaWebhooksTwitter200Response**

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

# **getMetaWebhooksTwitter**
> GetMetaWebhooksTwitter200Response getMetaWebhooksTwitter()

Get a list of all available subscriptions. 

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

const { status, data } = await apiInstance.getMetaWebhooksTwitter();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**GetMetaWebhooksTwitter200Response**

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

# **getWebhooksAlmanaxId**
> AlmanaxWebhook getWebhooksAlmanaxId()

Retrieve details about an existing Almanax Webhook with a given uuid.

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)

const { status, data } = await apiInstance.getWebhooksAlmanaxId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

**AlmanaxWebhook**

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

# **getWebhooksRssId**
> RssWebhook getWebhooksRssId()

Retrieve details about an existing RSS Webhook with a given uuid.

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)

const { status, data } = await apiInstance.getWebhooksRssId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

**RssWebhook**

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

# **getWebhooksTwitterId**
> TwitterWebhook getWebhooksTwitterId()

Retrieve details about an existing Twitter Webhook with a given uuid.

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)

const { status, data } = await apiInstance.getWebhooksTwitterId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

**TwitterWebhook**

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

# **postWebhooksAlmanax**
> postWebhooksAlmanax()

Register a new Webhook to post Almanax updates.

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    CreateAlmanaxWebhook
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let createAlmanaxWebhook: CreateAlmanaxWebhook; // (optional)

const { status, data } = await apiInstance.postWebhooksAlmanax(
    createAlmanaxWebhook
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAlmanaxWebhook** | **CreateAlmanaxWebhook**|  | |


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **postWebhooksRss**
> postWebhooksRss()

Register a new Webhook to post RSS news as soon as they are posted.

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    CreateRSSWebhook
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let createRSSWebhook: CreateRSSWebhook; // (optional)

const { status, data } = await apiInstance.postWebhooksRss(
    createRSSWebhook
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createRSSWebhook** | **CreateRSSWebhook**|  | |


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **postWebhooksTwitter**
> postWebhooksTwitter()

Register a new Webhook to post Twitter updates as soon as they are posted.

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    CreateTwitterWebhook
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let createTwitterWebhook: CreateTwitterWebhook; // (optional)

const { status, data } = await apiInstance.postWebhooksTwitter(
    createTwitterWebhook
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTwitterWebhook** | **CreateTwitterWebhook**|  | |


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **putWebhooksAlmanaxId**
> AlmanaxWebhook putWebhooksAlmanaxId()

Update the details of an Almanax Webhook. All fields are optional and arrays will be overwritten, so always put all selected items of an array.

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    PutAlmanaxWebhook
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)
let putAlmanaxWebhook: PutAlmanaxWebhook; // (optional)

const { status, data } = await apiInstance.putWebhooksAlmanaxId(
    id,
    putAlmanaxWebhook
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **putAlmanaxWebhook** | **PutAlmanaxWebhook**|  | |
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

**AlmanaxWebhook**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **putWebhooksRssId**
> RssWebhook putWebhooksRssId()

Update the details of a RSS Webhook. All fields are optional and arrays will be overwritten, so always put all selected items of an array.

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    PutRSSWebhook
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)
let putRSSWebhook: PutRSSWebhook; // (optional)

const { status, data } = await apiInstance.putWebhooksRssId(
    id,
    putRSSWebhook
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **putRSSWebhook** | **PutRSSWebhook**|  | |
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

**RssWebhook**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **putWebhooksTwitterId**
> TwitterWebhook putWebhooksTwitterId()

Update the details of a Twitter Webhook. All fields are optional and arrays will be overwritten, so always put all selected items of an array.

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    PutTwitterWebhook
} from 'dofusdude-ts';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let id: string; //the ID returned from the API when creating the webhook (default to undefined)
let putTwitterWebhook: PutTwitterWebhook; // (optional)

const { status, data } = await apiInstance.putWebhooksTwitterId(
    id,
    putTwitterWebhook
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **putTwitterWebhook** | **PutTwitterWebhook**|  | |
| **id** | [**string**] | the ID returned from the API when creating the webhook | defaults to undefined|


### Return type

**TwitterWebhook**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

