# Database Service

<b id="httpsopen-metadata.orgschemaentityservicesdatabaseservice.json">&#36;id: https://open-metadata.org/schema/entity/services/databaseService.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/services/databaseService.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/services/databaseService.json/properties/name">name</b> `required`
	 - Type: `string`
	 - Length: between 1 and 64
 - <b id="#https://open-metadata.org/schema/entity/services/databaseService.json/properties/serviceType">serviceType</b> `required`
	 - &#36;ref: [#/definitions/databaseServiceType](#/definitions/databaseServiceType)
 - <b id="#https://open-metadata.org/schema/entity/services/databaseService.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/services/databaseService.json/properties/href">href</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/services/databaseService.json/properties/jdbc">jdbc</b> `required`
	 - &#36;ref: [../../type/jdbcConnection.json#/definitions/jdbcInfo](#....typejdbcconnection.jsondefinitionsjdbcinfo)
 - <b id="#https://open-metadata.org/schema/entity/services/databaseService.json/properties/ingestionSchedule">ingestionSchedule</b>
	 - &#36;ref: [../../type/schedule.json](#....typeschedule.json)


## Type definitions in this schema
**databaseServiceType**

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


