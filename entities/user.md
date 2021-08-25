# User

<b id="httpsopen-metadata.orgschemaentityteamsuser.json">&#36;id: https://open-metadata.org/schema/entity/teams/user.json</b>

Type: `object`

This schema <u>does not</u> accept additional properties.

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)
 - **name** `required`
	 - &#36;ref: [#/definitions/userName](definitionsusername)
 - **displayName**
	 - Type: `string`
 - **email** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/email](....typebasic.mddefinitionsemail)
 - **href** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/href](....typebasic.mddefinitionshref)
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
	 - &#36;ref: [../../type/profile.json](....typeprofile.md)
 - **teams**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](....typeentityreference.mddefinitionsentityreferencelist)
 - **owns**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](....typeentityreference.mddefinitionsentityreferencelist)
 - **follows**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](....typeentityreference.mddefinitionsentityreferencelist)


## Type definitions in this schema
### userName

 - Type: `string`
 - Length: between 1 and 64


