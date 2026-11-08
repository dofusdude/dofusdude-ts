# MonsterGradeSpellsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ankama_id** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**grade** | **number** | The spell grade assigned to this monster grade. | [default to undefined]
**url** | **string** | URL for the assigned spell grade. Includes the &#x60;grade&#x60; query parameter. | [default to undefined]
**image_urls** | [**Images**](Images.md) |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**icon_id** | **number** |  | [optional] [default to undefined]
**admin_name** | **string** |  | [optional] [default to undefined]
**order** | **number** |  | [optional] [default to undefined]
**type** | [**CombatReference**](CombatReference.md) |  | [optional] [default to undefined]
**classes** | [**Array&lt;CombatReference&gt;**](CombatReference.md) |  | [optional] [default to undefined]
**monsters** | [**Array&lt;CombatReference&gt;**](CombatReference.md) |  | [optional] [default to undefined]
**levels** | [**Array&lt;SpellLevel&gt;**](SpellLevel.md) |  | [default to undefined]
**scripts** | [**Array&lt;SpellScriptUsage&gt;**](SpellScriptUsage.md) |  | [optional] [default to undefined]
**critical_scripts** | [**Array&lt;SpellScriptUsage&gt;**](SpellScriptUsage.md) |  | [optional] [default to undefined]

## Example

```typescript
import { MonsterGradeSpellsInner } from 'dofusdude-ts';

const instance: MonsterGradeSpellsInner = {
    ankama_id,
    name,
    grade,
    url,
    image_urls,
    description,
    icon_id,
    admin_name,
    order,
    type,
    classes,
    monsters,
    levels,
    scripts,
    critical_scripts,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
