# Topic

<b id="https/open-metadata.org/schema/entity/data/topic.json">&#36;id: https://open-metadata.org/schema/entity/data/topic.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **name** `required`
	 - &#36;ref: [#/definitions/topicName](#topicname)
 - **fullyQualifiedName**
	 - Type: `string`
 - **description**
	 - Type: `string`
 - **service** `required`
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **partitions** `required`
	 - Type: `integer`
	 - Range:  &ge; 1
 - **schemaText**
	 - Type: `string`
 - **schemaType**
	 - &#36;ref: [#/definitions/schemaType](#schematype)
 - **cleanupPolicies**
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/cleanupPolicy](#cleanuppolicy)
 - **retentionTime**
	 - Type: `number`
 - **maximumMessageSize**
	 - Type: `integer`
 - **minimumInSyncReplicas**
	 - Type: `integer`
 - **retentionSize**
	 - Type: `number`
	 - Default: _"-1"_
 - **owner**
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **followers**
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)
 - **tags**
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [../../type/tagLabel.json](../types/taglabel.md)
 - **href**
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)


## Type definitions in this schema
### topicName

 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


### schemaType

 - The value is restricted to the following: 
	 1. _"Avro"_
	 2. _"Protobuf"_
	 3. _"JSON"_
	 4. _"Other"_


### cleanupPolicy

 - The value is restricted to the following: 
	 1. _"delete"_
	 2. _"compact"_


