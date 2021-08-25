# Database

<b id="https/open-metadata.org/schema/entity/data/database.json">&#36;id: https://open-metadata.org/schema/entity/data/database.json </b>

Type: `object`

## Properties
### id
 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
### name `required`
 - &#36;ref: [#/definitions/databaseName](#databasename)
### fullyQualifiedName
Type: `string`

### description
Type: `string`

### href
 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
### owner
 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
### service `required`
 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
### usageSummary
 - &#36;ref: [../../type/usageDetails.json](../types/usagedetails.md)
### tables
 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)


## Type definitions in this schema
### databaseName

Type: `string`

 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


