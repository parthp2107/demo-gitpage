# Audit Log

<b id="httpsopen-metadata.orgschematypeauditlog.json">&#36;id: https://open-metadata.org/schema/type/auditLog.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/type/auditLog.json/properties/method">method</b> `required`
	 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"POST"_
		 2. _"PUT"_
		 3. _"PATCH"_
		 4. _"DELETE"_
 - <b id="#https://open-metadata.org/schema/type/auditLog.json/properties/responseCode">responseCode</b> `required`
	 - Type: `integer`
 - <b id="#https://open-metadata.org/schema/type/auditLog.json/properties/path">path</b> `required`
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/type/auditLog.json/properties/userName">userName</b> `required`
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/type/auditLog.json/properties/dateTime">dateTime</b>
	 - &#36;ref: [basic.json#/definitions/dateTime](#basic.jsondefinitionsdatetime)
 - <b id="#https://open-metadata.org/schema/type/auditLog.json/properties/entityId">entityId</b> `required`
	 - &#36;ref: [basic.json#/definitions/uuid](#basic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/type/auditLog.json/properties/entityType">entityType</b> `required`
	 - Type: `string`
