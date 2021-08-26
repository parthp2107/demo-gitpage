# JDBC connection

This schema defines the type used for JDBC connection information.

<b id="https/open-metadata.org/schema/type/jdbcconnection.json">&#36;id: https://open-metadata.org/schema/type/jdbcConnection.json</b>

Type: `object`

## Properties
 - **driverClass** `required`
	 - JDBC driver class.
	 - $ref: [#/definitions/driverClass](#driverclass)
 - **connectionUrl** `required`
	 - JDBC connection URL.
	 - $ref: [#/definitions/connectionUrl](#connectionurl)
 - **userName** `required`
	 - Login user name.
	 - Type: `string`
 - **password** `required`
	 - Login password.
	 - Type: `string`


## Type definitions in this schema
### driverClass

 - Type used for JDBC driver class.
 - Type: `string`


### connectionUrl

 - Type used for JDBC connection URL.
 - Type: `string`
 - String format must be a "uri"


### jdbcInfo

 - Type for capturing JDBC connector information.
 - Type: `object`
 - **Properties**
	 - **driverClass** `required`
		 - $ref: [#/definitions/driverClass](#driverclass)
	 - **connectionUrl** `required`
		 - $ref: [#/definitions/connectionUrl](#connectionurl)




_This Document was generated on: Thursday, August 26, 2021_