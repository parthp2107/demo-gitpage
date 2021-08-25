# JDBC connection

<b id="https/open-metadata.org/schema/type/jdbcconnection.json">&#36;id: https://open-metadata.org/schema/type/jdbcConnection.json </b>

Type: `object`

## Properties
### driverClass `required`
 - &#36;ref: [#/definitions/driverClass](#driverclass)
### connectionUrl `required`
 - &#36;ref: [#/definitions/connectionUrl](#connectionurl)
### userName `required`
Type: `string`

### password `required`
Type: `string`



## Type definitions in this schema
### driverClass

Type: `string`



### connectionUrl

Type: `string`

 - String format must be a "uri"


### jdbcInfo

Type: `object`

### Properties
 - ### driverClass `required`
	 - &#36;ref: [#/definitions/driverClass](#driverclass)
 - ### connectionUrl `required`
	 - &#36;ref: [#/definitions/connectionUrl](#connectionurl)


