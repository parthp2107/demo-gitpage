# User

<b id="https/open-metadata.org/schema/entity/teams/user.json">&#36;id: https://open-metadata.org/schema/entity/teams/user.json</b>

Type: `object`

This schema <u>does not</u> accept additional properties.

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **name** `required`
	 - &#36;ref: [#/definitions/userName](#username)
 - **displayName**
	 - Type: `string`
 - **email** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/email](../types/basic.md#email)
 - **href** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **timezone**
	 - Type: `string`
	 - String format must be a "timezone"
 - **deactivated**
	 - Type: `boolean`
 - **isBot**
	 - Type: `boolean`
 - **isAdmin**
	 - Type: `boolean`
 - **profile**
	 - &#36;ref: [../../type/profile.json](../types/profile.md)
 - **teams**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)
 - **owns**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)
 - **follows**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)


## Type definitions in this schema
### userName

 - Type: `string`
 - Length: between 1 and 64


