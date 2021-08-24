# Messaging Service

<b id="httpsopen-metadata.orgschemaentityservicesmessagingservice.json">&#36;id: https://open-metadata.org/schema/entity/services/messagingService.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/name">name</b> `required`
	 - Type: `string`
	 - Length: between 1 and 64
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/serviceType">serviceType</b> `required`
	 - &#36;ref: [#/definitions/messagingServiceType](#/definitions/messagingServiceType)
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/brokers">brokers</b> `required`
	 - &#36;ref: [#/definitions/brokers](#/definitions/brokers)
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/schemaRegistry">schemaRegistry</b>
	 - Type: `string`
	 - String format must be a "uri"
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/ingestionSchedule">ingestionSchedule</b>
	 - &#36;ref: [../../type/schedule.json](#....typeschedule.json)
 - <b id="#https://open-metadata.org/schema/entity/services/messagingService.json/properties/href">href</b>
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)


## Type definitions in this schema
**messagingServiceType**

 - Type: `string`
 - The value is restricted to the following: 
	 1. _"Kafka"_
	 2. _"Pulsar"_


**brokers**

 - Type: `array`
	 - **Items**
	 - Type: `string`


