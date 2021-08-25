# Messaging Service

<b id="https/open-metadata.org/schema/entity/services/messagingservice.json">&#36;id: https://open-metadata.org/schema/entity/services/messagingService.json </b>

Type: `object`

## Properties
### id `required`
 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
### name `required`
Type: `string`

 - Length: between 1 and 64
### serviceType `required`
 - &#36;ref: [#/definitions/messagingServiceType](#messagingservicetype)
### description
Type: `string`

### brokers `required`
 - &#36;ref: [#/definitions/brokers](#brokers)
### schemaRegistry
Type: `string`

 - String format must be a "uri"
### ingestionSchedule
 - &#36;ref: [../../type/schedule.json](../types/schedule.md)
### href
 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)


## Type definitions in this schema
### messagingServiceType

Type: `string`

 - The value is restricted to the following: 
	 1. _"Kafka"_
	 2. _"Pulsar"_


### brokers

Type: `array`

### Items
Type: `string`



