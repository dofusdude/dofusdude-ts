## dofusdude-ts@1.0.0

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install dofusdude-ts@1.0.0 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *https://api.dofusdu.de*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AlmanaxApi* | [**getAlmanaxDate**](docs/AlmanaxApi.md#getalmanaxdate) | **GET** /dofus3/v1/{language}/almanax/{date} | Single Almanax Date
*AlmanaxApi* | [**getAlmanaxRange**](docs/AlmanaxApi.md#getalmanaxrange) | **GET** /dofus3/v1/{language}/almanax | Almanax Range
*ConsumablesApi* | [**getAllItemsConsumablesList**](docs/ConsumablesApi.md#getallitemsconsumableslist) | **GET** /{game}/v1/{language}/items/consumables/all | List All Consumables
*ConsumablesApi* | [**getItemsConsumablesList**](docs/ConsumablesApi.md#getitemsconsumableslist) | **GET** /{game}/v1/{language}/items/consumables | List Consumables
*ConsumablesApi* | [**getItemsConsumablesSearch**](docs/ConsumablesApi.md#getitemsconsumablessearch) | **GET** /{game}/v1/{language}/items/consumables/search | Search Consumables
*ConsumablesApi* | [**getItemsConsumablesSingle**](docs/ConsumablesApi.md#getitemsconsumablessingle) | **GET** /{game}/v1/{language}/items/consumables/{ankama_id} | Single Consumables
*CosmeticsApi* | [**getAllCosmeticsList**](docs/CosmeticsApi.md#getallcosmeticslist) | **GET** /{game}/v1/{language}/items/cosmetics/all | List All Cosmetics
*CosmeticsApi* | [**getCosmeticsList**](docs/CosmeticsApi.md#getcosmeticslist) | **GET** /{game}/v1/{language}/items/cosmetics | List Cosmetics
*CosmeticsApi* | [**getCosmeticsSearch**](docs/CosmeticsApi.md#getcosmeticssearch) | **GET** /{game}/v1/{language}/items/cosmetics/search | Search Cosmetics
*CosmeticsApi* | [**getCosmeticsSingle**](docs/CosmeticsApi.md#getcosmeticssingle) | **GET** /{game}/v1/{language}/items/cosmetics/{ankama_id} | Single Cosmetics
*EquipmentApi* | [**getAllItemsEquipmentList**](docs/EquipmentApi.md#getallitemsequipmentlist) | **GET** /{game}/v1/{language}/items/equipment/all | List All Equipment
*EquipmentApi* | [**getItemsEquipmentList**](docs/EquipmentApi.md#getitemsequipmentlist) | **GET** /{game}/v1/{language}/items/equipment | List Equipment
*EquipmentApi* | [**getItemsEquipmentSearch**](docs/EquipmentApi.md#getitemsequipmentsearch) | **GET** /{game}/v1/{language}/items/equipment/search | Search Equipment
*EquipmentApi* | [**getItemsEquipmentSingle**](docs/EquipmentApi.md#getitemsequipmentsingle) | **GET** /{game}/v1/{language}/items/equipment/{ankama_id} | Single Equipment
*GameApi* | [**getGameSearch**](docs/GameApi.md#getgamesearch) | **GET** /{game}/v1/{language}/search | Game Search
*GameApi* | [**getItemsAllSearch**](docs/GameApi.md#getitemsallsearch) | **GET** /{game}/v1/{language}/items/search | Search All Items
*MetaApi* | [**getGameSearchTypes**](docs/MetaApi.md#getgamesearchtypes) | **GET** /{game}/v1/meta/search/types | Available Game Search Types
*MetaApi* | [**getItemTypes**](docs/MetaApi.md#getitemtypes) | **GET** /{game}/v1/meta/items/types | Available Item Types
*MetaApi* | [**getMetaAlmanaxBonuses**](docs/MetaApi.md#getmetaalmanaxbonuses) | **GET** /dofus3/v1/meta/{language}/almanax/bonuses | Available Almanax Bonuses
*MetaApi* | [**getMetaAlmanaxBonusesSearch**](docs/MetaApi.md#getmetaalmanaxbonusessearch) | **GET** /dofus3/v1/meta/{language}/almanax/bonuses/search | Search Available Almanax Bonuses
*MetaApi* | [**getMetaElements**](docs/MetaApi.md#getmetaelements) | **GET** /{game}/v1/meta/elements | Effects and Condition Elements
*MetaApi* | [**getMetaVersion**](docs/MetaApi.md#getmetaversion) | **GET** /{game}/v1/meta/version | Game Version
*MountsApi* | [**getAllMountsList**](docs/MountsApi.md#getallmountslist) | **GET** /{game}/v1/{language}/mounts/all | List All Mounts
*MountsApi* | [**getMountsList**](docs/MountsApi.md#getmountslist) | **GET** /{game}/v1/{language}/mounts | List Mounts
*MountsApi* | [**getMountsSearch**](docs/MountsApi.md#getmountssearch) | **GET** /{game}/v1/{language}/mounts/search | Search Mounts
*MountsApi* | [**getMountsSingle**](docs/MountsApi.md#getmountssingle) | **GET** /{game}/v1/{language}/mounts/{ankama_id} | Single Mounts
*QuestItemsApi* | [**getAllItemsQuestList**](docs/QuestItemsApi.md#getallitemsquestlist) | **GET** /{game}/v1/{language}/items/quest/all | List All Quest Items
*QuestItemsApi* | [**getItemQuestSingle**](docs/QuestItemsApi.md#getitemquestsingle) | **GET** /{game}/v1/{language}/items/quest/{ankama_id} | Single Quest Items
*QuestItemsApi* | [**getItemsQuestList**](docs/QuestItemsApi.md#getitemsquestlist) | **GET** /{game}/v1/{language}/items/quest | List Quest Items
*QuestItemsApi* | [**getItemsQuestSearch**](docs/QuestItemsApi.md#getitemsquestsearch) | **GET** /{game}/v1/{language}/items/quest/search | Search Quest Items
*ResourcesApi* | [**getAllItemsResourcesList**](docs/ResourcesApi.md#getallitemsresourceslist) | **GET** /{game}/v1/{language}/items/resources/all | List All Resources
*ResourcesApi* | [**getItemsResourceSearch**](docs/ResourcesApi.md#getitemsresourcesearch) | **GET** /{game}/v1/{language}/items/resources/search | Search Resources
*ResourcesApi* | [**getItemsResourcesList**](docs/ResourcesApi.md#getitemsresourceslist) | **GET** /{game}/v1/{language}/items/resources | List Resources
*ResourcesApi* | [**getItemsResourcesSingle**](docs/ResourcesApi.md#getitemsresourcessingle) | **GET** /{game}/v1/{language}/items/resources/{ankama_id} | Single Resources
*SetsApi* | [**getAllSetsList**](docs/SetsApi.md#getallsetslist) | **GET** /{game}/v1/{language}/sets/all | List All Sets
*SetsApi* | [**getSetsList**](docs/SetsApi.md#getsetslist) | **GET** /{game}/v1/{language}/sets | List Sets
*SetsApi* | [**getSetsSearch**](docs/SetsApi.md#getsetssearch) | **GET** /{game}/v1/{language}/sets/search | Search Sets
*SetsApi* | [**getSetsSingle**](docs/SetsApi.md#getsetssingle) | **GET** /{game}/v1/{language}/sets/{ankama_id} | Single Sets
*WebhooksApi* | [**deleteWebhooksAlmanaxId**](docs/WebhooksApi.md#deletewebhooksalmanaxid) | **DELETE** /webhooks/almanax/{id} | Unregister Almanax Hook
*WebhooksApi* | [**deleteWebhooksRssId**](docs/WebhooksApi.md#deletewebhooksrssid) | **DELETE** /webhooks/rss/{id} | Unregister RSS Hook
*WebhooksApi* | [**deleteWebhooksTwitterId**](docs/WebhooksApi.md#deletewebhookstwitterid) | **DELETE** /webhooks/twitter/{id} | Unregister Twitter Hook
*WebhooksApi* | [**getMetaWebhooksAlmanax**](docs/WebhooksApi.md#getmetawebhooksalmanax) | **GET** /meta/webhooks/almanax | Get Almanax Hook Metainfo
*WebhooksApi* | [**getMetaWebhooksRss**](docs/WebhooksApi.md#getmetawebhooksrss) | **GET** /meta/webhooks/rss | Get RSS Hook Metainfo
*WebhooksApi* | [**getMetaWebhooksTwitter**](docs/WebhooksApi.md#getmetawebhookstwitter) | **GET** /meta/webhooks/twitter | Get Twitter Hook Metainfo
*WebhooksApi* | [**getWebhooksAlmanaxId**](docs/WebhooksApi.md#getwebhooksalmanaxid) | **GET** /webhooks/almanax/{id} | Get Almanax Hook
*WebhooksApi* | [**getWebhooksRssId**](docs/WebhooksApi.md#getwebhooksrssid) | **GET** /webhooks/rss/{id} | Get RSS Hook
*WebhooksApi* | [**getWebhooksTwitterId**](docs/WebhooksApi.md#getwebhookstwitterid) | **GET** /webhooks/twitter/{id} | Get Twitter Hook
*WebhooksApi* | [**postWebhooksAlmanax**](docs/WebhooksApi.md#postwebhooksalmanax) | **POST** /webhooks/almanax | Register Almanax Hook
*WebhooksApi* | [**postWebhooksRss**](docs/WebhooksApi.md#postwebhooksrss) | **POST** /webhooks/rss | Register RSS Hook
*WebhooksApi* | [**postWebhooksTwitter**](docs/WebhooksApi.md#postwebhookstwitter) | **POST** /webhooks/twitter | Register Twitter Hook
*WebhooksApi* | [**putWebhooksAlmanaxId**](docs/WebhooksApi.md#putwebhooksalmanaxid) | **PUT** /webhooks/almanax/{id} | Update Almanax Hook
*WebhooksApi* | [**putWebhooksRssId**](docs/WebhooksApi.md#putwebhooksrssid) | **PUT** /webhooks/rss/{id} | Update RSS Hook
*WebhooksApi* | [**putWebhooksTwitterId**](docs/WebhooksApi.md#putwebhookstwitterid) | **PUT** /webhooks/twitter/{id} | Update Twitter Hook


### Documentation For Models

 - [Almanax](docs/Almanax.md)
 - [AlmanaxBonus](docs/AlmanaxBonus.md)
 - [AlmanaxTribute](docs/AlmanaxTribute.md)
 - [AlmanaxTributeItem](docs/AlmanaxTributeItem.md)
 - [AlmanaxWebhook](docs/AlmanaxWebhook.md)
 - [AlmanaxWebhookDailySettings](docs/AlmanaxWebhookDailySettings.md)
 - [Condition](docs/Condition.md)
 - [ConditionLeaf](docs/ConditionLeaf.md)
 - [ConditionNode](docs/ConditionNode.md)
 - [ConditionRelation](docs/ConditionRelation.md)
 - [CreateAlmanaxWebhook](docs/CreateAlmanaxWebhook.md)
 - [CreateAlmanaxWebhookDailySettings](docs/CreateAlmanaxWebhookDailySettings.md)
 - [CreateAlmanaxWebhookMentionsValueInner](docs/CreateAlmanaxWebhookMentionsValueInner.md)
 - [CreateRSSWebhook](docs/CreateRSSWebhook.md)
 - [CreateTwitterWebhook](docs/CreateTwitterWebhook.md)
 - [Effect](docs/Effect.md)
 - [EffectType](docs/EffectType.md)
 - [Equipment](docs/Equipment.md)
 - [EquipmentSet](docs/EquipmentSet.md)
 - [GameSearch](docs/GameSearch.md)
 - [GameSearchItem](docs/GameSearchItem.md)
 - [GameSearchType](docs/GameSearchType.md)
 - [GetMetaAlmanaxBonuses200ResponseInner](docs/GetMetaAlmanaxBonuses200ResponseInner.md)
 - [GetMetaWebhooksTwitter200Response](docs/GetMetaWebhooksTwitter200Response.md)
 - [Images](docs/Images.md)
 - [ItemSubtype](docs/ItemSubtype.md)
 - [ListEquipmentSet](docs/ListEquipmentSet.md)
 - [ListEquipmentSets](docs/ListEquipmentSets.md)
 - [ListItem](docs/ListItem.md)
 - [ListItemGeneral](docs/ListItemGeneral.md)
 - [ListItems](docs/ListItems.md)
 - [ListMounts](docs/ListMounts.md)
 - [ModelError](docs/ModelError.md)
 - [Mount](docs/Mount.md)
 - [MountFamily](docs/MountFamily.md)
 - [PagedLinks](docs/PagedLinks.md)
 - [PutAlmanaxWebhook](docs/PutAlmanaxWebhook.md)
 - [PutRSSWebhook](docs/PutRSSWebhook.md)
 - [PutTwitterWebhook](docs/PutTwitterWebhook.md)
 - [Range](docs/Range.md)
 - [Recipe](docs/Recipe.md)
 - [Resource](docs/Resource.md)
 - [RssWebhook](docs/RssWebhook.md)
 - [TranslatedId](docs/TranslatedId.md)
 - [TwitterWebhook](docs/TwitterWebhook.md)
 - [Version](docs/Version.md)
 - [Weapon](docs/Weapon.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization

Endpoints do not require authorization.

