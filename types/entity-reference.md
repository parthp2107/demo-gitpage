# Entity Reference

<b id="httpsopen-metadata.orgschematypeentityreference.json">&#36;id: https://open-metadata.org/schema/type/entityReference.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/type/entityReference.json/properties/id">id</b> `required`
	 - &#36;ref: [basic.json#/definitions/uuid](#basic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/type/entityReference.json/properties/type">type</b> `required`
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/type/entityReference.json/properties/name">name</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/type/entityReference.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/type/entityReference.json/properties/href">href</b>
	 - &#36;ref: [basic.json#/definitions/href](#basic.jsondefinitionshref)


## Type definitions in this schema
**entityReferenceList**

 - Type: `array`
	 - **Items**
	 - &#36;ref: [entityReference.json](#entityreference.json)


