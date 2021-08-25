# Audit Log

<b id="https/open-metadata.org/schema/type/auditlog.json">&#36;id: https://open-metadata.org/schema/type/auditLog.json</b>

Type: `object`

## Properties
 - **method** `required`
	 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"POST"_
		 2. _"PUT"_
		 3. _"PATCH"_
		 4. _"DELETE"_
 - **responseCode** `required`
	 - Type: `integer`
 - **path** `required`
	 - Type: `string`
 - **userName** `required`
	 - Type: `string`
 - **dateTime**
	 - &#36;ref: [basic.json#/definitions/dateTime](basic.md#datetime)
 - **entityId** `required`
	 - &#36;ref: [basic.json#/definitions/uuid](basic.md#uuid)
 - **entityType** `required`
	 - Type: `string`
