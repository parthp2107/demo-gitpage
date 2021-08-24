# User

<b id="httpsopen-metadata.orgschemaentityteamsuser.json">&#36;id: https://open-metadata.org/schema/entity/teams/user.json</b>

Type: `object`

This schema <u>does not</u> accept additional properties.

## Properties
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/name">name</b> `required`
	 - &#36;ref: [#/definitions/userName](#/definitions/userName)
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/displayName">displayName</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/email">email</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/email](#....typebasic.jsondefinitionsemail)
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/href">href</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/timezone">timezone</b>
	 - Type: `string`
	 - String format must be a "timezone"
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/deactivated">deactivated</b>
	 - Type: `boolean`
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/isBot">isBot</b>
	 - Type: `boolean`
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/isAdmin">isAdmin</b>
	 - Type: `boolean`
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/profile">profile</b>
	 - &#36;ref: [../../type/profile.json](#....typeprofile.json)
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/teams">teams</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/owns">owns</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)
 - <b id="#https://open-metadata.org/schema/entity/teams/user.json/properties/follows">follows</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)


## Type definitions in this schema
**userName**

 - Type: `string`
 - Length: between 1 and 64


