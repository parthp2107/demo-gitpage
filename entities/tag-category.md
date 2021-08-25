# Tag Category

This schema defines the Tag Category entity. A Tag Category contains tags called Primary Tags. Primary Tags can further have children Tags called Secondary Tags. Only two levels of tags are supported currently.

<b id="https/open-metadata.org/schema/entity/tags/tagcategory.json">&#36;id: https://open-metadata.org/schema/entity/tags/tagCategory.json</b>

Type: `object`

This schema <u>does not</u> accept additional properties.

## Properties
 - **name** `required`
	 - &#36;ref: [#/definitions/tagName](#tagname)
 - **description** `required`
	 - Description of the tag category.
	 - Type: `string`
 - **categoryType** `required`
	 - &#36;ref: [#/definitions/tagCategoryType](#tagcategorytype)
 - **href**
	 - Link to the resource corresponding to the tag category.
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **usageCount**
	 - Count of how many times the tags from this tag category are used.
	 - Type: `integer`
 - **children**
	 - Tags under this category.
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/tag](#tag)


## Type definitions in this schema
### tagName

 - Name of the tag.
 - Type: `string`
 - Length: between 2 and 25


### tagCategoryType

 - Type of tag category.
 - Type: `string`
 - The value is restricted to the following: 
	 1. _"Descriptive"_
	 2. _"Classification"_


### tag



