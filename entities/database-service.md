# Database Service

<b id="httpsopen-metadata.orgschemaentityservicesdatabaseservice.json">&#36;id: https://open-metadata.org/schema/entity/services/databaseService.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)
 - **name** `required`
	 - Type: `string`
	 - Length: between 1 and 64
 - **serviceType** `required`
	 - &#36;ref: [#/definitions/databaseServiceType](definitionsdatabaseservicetype)
 - **description**
	 - Type: `string`
 - **href** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/href](....typebasic.mddefinitionshref)
 - **jdbc** `required`
	 - &#36;ref: [../../type/jdbcConnection.json#/definitions/jdbcInfo](....typejdbcconnection.mddefinitionsjdbcinfo)
 - **ingestionSchedule**
	 - &#36;ref: [../../type/schedule.json](....typeschedule.md)


## Type definitions in this schema
### databaseServiceType

 - Type: `string`
 - The value is restricted to the following: 
	 1. _"BigQuery"_
	 2. _"MySQL"_
	 3. _"Redshift"_
	 4. _"Snowflake"_
	 5. _"Postgres"_
	 6. _"MSSQL"_
	 7. _"Hive"_
	 8. _"Oracle"_
	 9. _"Athena"_
	 10. _"Presto"_


