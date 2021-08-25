# Topic

This schema defines the Topic entity. A topic is a feed into which message are published to by publishers and read from by consumers in a messaging service.

<b id="https/open-metadata.org/schema/entity/data/topic.json">&#36;id: https://open-metadata.org/schema/entity/data/topic.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - Unique identifier that identifies this topic instance.
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **name** `required`
	 - Name that identifies the topic.
	 - &#36;ref: [#/definitions/topicName](#topicname)
 - **fullyQualifiedName**
	 - Name that uniquely identifies a topic in the format 'messagingServiceName.topicName'.
	 - Type: `string`
 - **description**
	 - Description of the topic instance.
	 - Type: `string`
 - **service** `required`
	 - Link to the messaging cluster/service where this topic is hosted in.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **partitions** `required`
	 - Number of partitions into which the topic is divided.
	 - Type: `integer`
	 - Range:  &ge; 1
 - **schemaText**
	 - Schema used for message serialization. Optional as some topics may not have associated schemas.
	 - Type: `string`
 - **schemaType**
	 - Schema used for message serialization.
	 - &#36;ref: [#/definitions/schemaType](#schematype)
 - **cleanupPolicies**
	 - Topic clean up policies. For Kafka - `cleanup.policy` configuration.
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/cleanupPolicy](#cleanuppolicy)
 - **retentionTime**
	 - Retention time in milliseconds. For Kafka - `retention.ms` configuration.
	 - Type: `number`
 - **maximumMessageSize**
	 - Maximum message size in bytes. For Kafka - `max.message.bytes` configuration.
	 - Type: `integer`
 - **minimumInSyncReplicas**
	 - Minimum number replicas in sync to control durability. For Kafka - `min.insync.replicas` configuration.
	 - Type: `integer`
 - **retentionSize**
	 - Maximum size of a partition in bytes before old data is discarded. For Kafka - `retention.bytes` configuration.
	 - Type: `number`
	 - Default: _"-1"_
 - **owner**
	 - Owner of this topic.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **followers**
	 - Followers of this table.
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)
 - **tags**
	 - Tags for this table.
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [../../type/tagLabel.json](../types/taglabel.md)
 - **href**
	 - Link to the resource corresponding to this entity.
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)


## Type definitions in this schema
### topicName

 - Name that identifies a topic.
 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


### schemaType

 - Schema type used for the message.
 - The value is restricted to the following: 
	 1. _"Avro"_
	 2. _"Protobuf"_
	 3. _"JSON"_
	 4. _"Other"_


### cleanupPolicy

 - Topic clean up policy. For Kafka - `cleanup.policy` configuration.
 - The value is restricted to the following: 
	 1. _"delete"_
	 2. _"compact"_


