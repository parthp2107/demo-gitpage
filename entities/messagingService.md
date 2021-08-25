# Messaging Service

<b id="httpsopen-metadata.orgschemaentityservicesmessagingservice.json">&#36;id: https://open-metadata.org/schema/entity/services/messagingService.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)
 - **name** `required`
	 - Type: `string`
	 - Length: between 1 and 64
 - **serviceType** `required`
	 - &#36;ref: [#/definitions/messagingServiceType](definitionsmessagingservicetype)
 - **description**
	 - Type: `string`
 - **brokers** `required`
	 - &#36;ref: [#/definitions/brokers](definitionsbrokers)
 - **schemaRegistry**
	 - Type: `string`
	 - String format must be a "uri"
 - **ingestionSchedule**
	 - &#36;ref: [../../type/schedule.json](....typeschedule.md)
 - **href**
	 - &#36;ref: [../../type/basic.json#/definitions/href](....typebasic.mddefinitionshref)


## Type definitions in this schema
### messagingServiceType

 - Type: `string`
 - The value is restricted to the following: 
	 1. _"Kafka"_
	 2. _"Pulsar"_


### brokers

 - Type: `array`
	 - **Items**
	 - Type: `string`


