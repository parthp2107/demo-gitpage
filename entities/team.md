# Team

<b id="httpsopen-metadata.orgschemaentityteamsteam.json">&#36;id: https://open-metadata.org/schema/entity/teams/team.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/name">name</b> `required`
	 - &#36;ref: [#/definitions/teamName](#/definitions/teamName)
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/displayName">displayName</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/href">href</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/profile">profile</b>
	 - &#36;ref: [../../type/profile.json](#....typeprofile.json)
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/deleted">deleted</b>
	 - Type: `boolean`
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/users">users</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)
 - <b id="#https://open-metadata.org/schema/entity/teams/team.json/properties/owns">owns</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)


## Type definitions in this schema
**teamName**

 - Type: `string`
 - Length: between 1 and 64


