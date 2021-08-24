# Tag Category

<b id="httpsopen-metadata.orgschemaentitytagstagcategory.json">&#36;id: https://open-metadata.org/schema/entity/tags/tagCategory.json</b>

Type: `object`

This schema <u>does not</u> accept additional properties.

## Properties
 - <b id="#https://open-metadata.org/schema/entity/tags/tagCategory.json/properties/name">name</b> `required`
	 - &#36;ref: [#/definitions/tagName](#/definitions/tagName)
 - <b id="#https://open-metadata.org/schema/entity/tags/tagCategory.json/properties/description">description</b> `required`
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/tags/tagCategory.json/properties/categoryType">categoryType</b> `required`
	 - &#36;ref: [#/definitions/tagCategoryType](#/definitions/tagCategoryType)
 - <b id="#https://open-metadata.org/schema/entity/tags/tagCategory.json/properties/href">href</b>
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/tags/tagCategory.json/properties/usageCount">usageCount</b>
	 - Type: `integer`
 - <b id="#https://open-metadata.org/schema/entity/tags/tagCategory.json/properties/children">children</b>
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/tag](#/definitions/tag)


## Type definitions in this schema
**tagName**

 - Type: `string`
 - Length: between 2 and 25


**tagCategoryType**

 - Type: `string`
 - The value is restricted to the following: 
	 1. _"Descriptive"_
	 2. _"Classification"_


**tag**



