# Database

This schema defines the Database entity. A database also referred to as Database Catalog is a collection of tables.

<b id="https/open-metadata.org/schema/entity/data/database.json">&#36;id: https://open-metadata.org/schema/entity/data/database.json</b>

Type: `object`

## Properties
 - **id**
	 - Unique identifier that identifies this database instance.
	 - $ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **name** `required`
	 - Name that identifies the database.
	 - $ref: [#/definitions/databaseName](#databasename)
 - **fullyQualifiedName**
	 - Name that uniquely identifies a database in the format 'ServiceName.DatabaseName'.
	 - Type: `string`
 - **description**
	 - Description of the database instance.
	 - Type: `string`
 - **href**
	 - Link to the resource corresponding to this entity.
	 - $ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **owner**
	 - Owner of this database.
	 - $ref: [../../type/entityReference.json](../types/entityreference.md)
 - **service** `required`
	 - Link to the database cluster/service where this database is hosted in.
	 - $ref: [../../type/entityReference.json](../types/entityreference.md)
 - **usageSummary**
	 - Latest usage information for this database.
	 - $ref: [../../type/usageDetails.json](../types/usagedetails.md)
 - **tables**
	 - References to tables in the database.
	 - $ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)


## Type definitions in this schema
### databaseName

 - Name that identifies the database.
 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64




_This Document was generated on: Thursday, August 26, 2021_