# Audit Log

This schema defines the Audit Log type to capture the audit trail of POST, PUT, and PATCH API operations.

<b id="https/open-metadata.org/schema/type/auditlog.json">&#36;id: https://open-metadata.org/schema/type/auditLog.json</b>

Type: `object`

## Properties
 - **method** `required`
	 - HTTP Method used in a call.
	 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"POST"_
		 2. _"PUT"_
		 3. _"PATCH"_
		 4. _"DELETE"_
 - **responseCode** `required`
	 - HTTP response code for the api requested.
	 - Type: `integer`
 - **path** `required`
	 - Requested API Path.
	 - Type: `string`
 - **userName** `required`
	 - Name of the user who made the API request.
	 - Type: `string`
 - **dateTime**
	 - Date when the API call is made.
	 - &#36;ref: [basic.json#/definitions/dateTime](basic.md#datetime)
 - **entityId** `required`
	 - Identifier of entity that was modified by the operation.
	 - &#36;ref: [basic.json#/definitions/uuid](basic.md#uuid)
 - **entityType** `required`
	 - Type of Entity that is modified by the operation.
	 - Type: `string`
