# Tag Category

<b id="https/open-metadata.org/schema/entity/tags/tagcategory.json">&#36;id: https://open-metadata.org/schema/entity/tags/tagCategory.json </b>

Type: `object`

This schema <u>does not</u> accept additional properties.

## Properties
### name `required`
 - &#36;ref: [#/definitions/tagName](#tagname)
### description `required`
Type: `string`

### categoryType `required`
 - &#36;ref: [#/definitions/tagCategoryType](#tagcategorytype)
### href
 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
### usageCount
Type: `integer`

### children
Type: `array`

### Items
&#36;ref: [#/definitions/tag](#tag)



## Type definitions in this schema
### tagName

Type: `string`

 - Length: between 2 and 25


### tagCategoryType

Type: `string`

 - The value is restricted to the following: 
	 1. _"Descriptive"_
	 2. _"Classification"_


### tag



