# JDBC connection

<b id="httpsopen-metadata.orgschematypejdbcconnection.json">&#36;id: https://open-metadata.org/schema/type/jdbcConnection.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/type/jdbcConnection.json/properties/driverClass">driverClass</b> `required`
	 - &#36;ref: [#/definitions/driverClass](#/definitions/driverClass)
 - <b id="#https://open-metadata.org/schema/type/jdbcConnection.json/properties/connectionUrl">connectionUrl</b> `required`
	 - &#36;ref: [#/definitions/connectionUrl](#/definitions/connectionUrl)
 - <b id="#https://open-metadata.org/schema/type/jdbcConnection.json/properties/userName">userName</b> `required`
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/type/jdbcConnection.json/properties/password">password</b> `required`
	 - Type: `string`


## Type definitions in this schema
**driverClass**

 - Type: `string`


**connectionUrl**

 - Type: `string`
 - String format must be a "uri"


**jdbcInfo**

 - Type: `object`
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/type/jdbcConnection.json/definitions/jdbcInfo/properties/driverClass">driverClass</b> `required`
		 - &#36;ref: [#/definitions/driverClass](#/definitions/driverClass)
	 - <b id="#https://open-metadata.org/schema/type/jdbcConnection.json/definitions/jdbcInfo/properties/connectionUrl">connectionUrl</b> `required`
		 - &#36;ref: [#/definitions/connectionUrl](#/definitions/connectionUrl)


