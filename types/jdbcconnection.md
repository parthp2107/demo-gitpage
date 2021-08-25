# JDBC connection

<b id="httpsopen-metadata.orgschematypejdbcconnection.json">&#36;id: https://open-metadata.org/schema/type/jdbcConnection.json</b>

Type: `object`

## Properties
 - **driverClass** `required`
	 - &#36;ref: [#/definitions/driverClass](definitionsdriverclass)
 - **connectionUrl** `required`
	 - &#36;ref: [#/definitions/connectionUrl](definitionsconnectionurl)
 - **userName** `required`
	 - Type: `string`
 - **password** `required`
	 - Type: `string`


## Type definitions in this schema
### driverClass

 - Type: `string`


### connectionUrl

 - Type: `string`
 - String format must be a "uri"


### jdbcInfo

 - Type: `object`
 - **Properties**
	 - **driverClass** `required`
		 - &#36;ref: [#/definitions/driverClass](definitionsdriverclass)
	 - **connectionUrl** `required`
		 - &#36;ref: [#/definitions/connectionUrl](definitionsconnectionurl)


