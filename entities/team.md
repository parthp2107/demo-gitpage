# Team

<b id="httpsopen-metadata.orgschemaentityteamsteam.json">&#36;id: https://open-metadata.org/schema/entity/teams/team.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)
 - **name** `required`
	 - &#36;ref: [#/definitions/teamName](definitionsteamname)
 - **displayName**
	 - Type: `string`
 - **description**
	 - Type: `string`
 - **href** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/href](....typebasic.mddefinitionshref)
 - **profile**
	 - &#36;ref: [../../type/profile.json](....typeprofile.md)
 - **deleted**
	 - Type: `boolean`
 - **users**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](....typeentityreference.mddefinitionsentityreferencelist)
 - **owns**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](....typeentityreference.mddefinitionsentityreferencelist)


## Type definitions in this schema
### teamName

 - Type: `string`
 - Length: between 1 and 64


