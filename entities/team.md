# Team

<b id="https/open-metadata.org/schema/entity/teams/team.json">&#36;id: https://open-metadata.org/schema/entity/teams/team.json </b>

Type: `object`

## Properties
### id `required`
 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
### name `required`
 - &#36;ref: [#/definitions/teamName](#teamname)
### displayName
Type: `string`

### description
Type: `string`

### href `required`
 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
### profile
 - &#36;ref: [../../type/profile.json](../types/profile.md)
### deleted
Type: `boolean`

### users
 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)
### owns
 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)


## Type definitions in this schema
### teamName

Type: `string`

 - Length: between 1 and 64


