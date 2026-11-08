# MappedEntityCollection

The populated array property matches the selected resource.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**classes** | [**Array&lt;MappedEntityCollectionClassesInner&gt;**](MappedEntityCollectionClassesInner.md) |  | [optional] [default to undefined]
**spells** | [**Array&lt;MappedEntityCollectionSpellsInner&gt;**](MappedEntityCollectionSpellsInner.md) |  | [optional] [default to undefined]
**monsters** | [**Array&lt;MappedEntityCollectionMonstersInner&gt;**](MappedEntityCollectionMonstersInner.md) |  | [optional] [default to undefined]
**super_areas** | [**Array&lt;MappedEntityCollectionSuperAreasInner&gt;**](MappedEntityCollectionSuperAreasInner.md) |  | [optional] [default to undefined]
**areas** | [**Array&lt;MappedEntityCollectionSuperAreasInner&gt;**](MappedEntityCollectionSuperAreasInner.md) |  | [optional] [default to undefined]
**subareas** | [**Array&lt;MappedEntityCollectionSuperAreasInner&gt;**](MappedEntityCollectionSuperAreasInner.md) |  | [optional] [default to undefined]
**_links** | **{ [key: string]: any; }** |  | [optional] [default to undefined]

## Example

```typescript
import { MappedEntityCollection } from 'dofusdude-ts';

const instance: MappedEntityCollection = {
    classes,
    spells,
    monsters,
    super_areas,
    areas,
    subareas,
    _links,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
