# Table

<b id="httpsopen-metadata.orgschemaentitydatatable.json">&#36;id: https://open-metadata.org/schema/entity/data/table.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/name">name</b> `required`
	 - &#36;ref: [#/definitions/tableName](#/definitions/tableName)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/href">href</b>
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/tableType">tableType</b>
	 - &#36;ref: [#/definitions/tableType](#/definitions/tableType)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/fullyQualifiedName">fullyQualifiedName</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/columns">columns</b> `required`
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/column](#/definitions/column)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/tableConstraints">tableConstraints</b>
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/tableConstraint](#/definitions/tableConstraint)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/usageSummary">usageSummary</b>
	 - &#36;ref: [../../type/usageDetails.json](#....typeusagedetails.json)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/owner">owner</b>
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/followers">followers</b>
	 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](#....typeentityreference.jsondefinitionsentityreferencelist)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/database">database</b>
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/viewDefinition">viewDefinition</b>
	 - &#36;ref: [../../type/basic.json#/definitions/sqlQuery](#....typebasic.jsondefinitionssqlquery)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/tags">tags</b>
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [../../type/tagLabel.json](#....typetaglabel.json)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/joins">joins</b>
	 - &#36;ref: [#/definitions/tableJoins](#/definitions/tableJoins)
 - <b id="#https://open-metadata.org/schema/entity/data/table.json/properties/sampleData">sampleData</b>
	 - &#36;ref: [#/definitions/tableData](#/definitions/tableData)


## Type definitions in this schema
**tableType**

 - Type: `string`
 - The value is restricted to the following: 
	 1. _"Regular"_
	 2. _"External"_
	 3. _"View"_
	 4. _"SecureView"_
	 5. _"MaterializedView"_


**columnDataType**

 - Type: `string`
 - The value is restricted to the following: 
	 1. _"NUMBER"_
	 2. _"TINYINT"_
	 3. _"SMALLINT"_
	 4. _"INT"_
	 5. _"BIGINT"_
	 6. _"FLOAT"_
	 7. _"DOUBLE"_
	 8. _"DECIMAL"_
	 9. _"NUMERIC"_
	 10. _"TIMESTAMP"_
	 11. _"TIME"_
	 12. _"DATE"_
	 13. _"DATETIME"_
	 14. _"INTERVAL"_
	 15. _"STRING"_
	 16. _"MEDIUMTEXT"_
	 17. _"TEXT"_
	 18. _"CHAR"_
	 19. _"VARCHAR"_
	 20. _"BOOLEAN"_
	 21. _"BINARY"_
	 22. _"VARBINARY"_
	 23. _"ARRAY"_
	 24. _"BLOB"_
	 25. _"LONGBLOB"_
	 26. _"MEDIUMBLOB"_
	 27. _"MAP"_
	 28. _"STRUCT"_
	 29. _"UNION"_
	 30. _"SET"_
	 31. _"GEOGRAPHY"_
	 32. _"ENUM"_
	 33. _"JSON"_


**columnConstraint**

 - Type: `string`
 - The value is restricted to the following: 
	 1. _"NULL"_
	 2. _"NOT_NULL"_
	 3. _"UNIQUE"_
	 4. _"PRIMARY_KEY"_
 - Default: _"NULL"_


**tableConstraint**

 - Type: `object`
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/tableConstraint/properties/constraintType">constraintType</b>
		 - Type: `string`
		 - The value is restricted to the following: 
			 1. _"UNIQUE"_
			 2. _"PRIMARY_KEY"_
			 3. _"FOREIGN_KEY"_
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/tableConstraint/properties/columns">columns</b>
		 - Type: `array`
			 - **Items**
			 - Type: `string`


**columnName**

 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


**tableName**

 - Type: `string`
 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


**fullyQualifiedColumnName**

 - Type: `string`
 - Length: between 1 and 256


**column**

 - Type: `object`
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/column/properties/name">name</b> `required`
		 - &#36;ref: [#/definitions/columnName](#/definitions/columnName)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/column/properties/columnDataType">columnDataType</b> `required`
		 - &#36;ref: [#/definitions/columnDataType](#/definitions/columnDataType)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/column/properties/description">description</b>
		 - Type: `string`
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/column/properties/fullyQualifiedName">fullyQualifiedName</b>
		 - &#36;ref: [#/definitions/fullyQualifiedColumnName](#/definitions/fullyQualifiedColumnName)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/column/properties/tags">tags</b>
		 - Type: `array`
			 - **Items**
			 - &#36;ref: [../../type/tagLabel.json](#....typetaglabel.json)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/column/properties/columnConstraint">columnConstraint</b>
		 - &#36;ref: [#/definitions/columnConstraint](#/definitions/columnConstraint)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/column/properties/ordinalPosition">ordinalPosition</b>
		 - Type: `integer`


**columnJoins**

 - Type: `object`
 - This schema <u>does not</u> accept additional properties.
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/columnJoins/properties/columnName">columnName</b>
		 - &#36;ref: [#/definitions/columnName](#/definitions/columnName)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/columnJoins/properties/joinedWith">joinedWith</b>
		 - Type: `array`
			 - **Items**
			 - Type: `object`
			 - **Properties**
				 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/columnJoins/properties/joinedWith/items/properties/fullyQualifiedName">fullyQualifiedName</b>
					 - &#36;ref: [#/definitions/fullyQualifiedColumnName](#/definitions/fullyQualifiedColumnName)
				 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/columnJoins/properties/joinedWith/items/properties/joinCount">joinCount</b>
					 - Type: `integer`


**tableJoins**

 - Type: `object`
 - This schema <u>does not</u> accept additional properties.
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/tableJoins/properties/startDate">startDate</b>
		 - &#36;ref: [../../type/basic.json#/definitions/date](#....typebasic.jsondefinitionsdate)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/tableJoins/properties/dayCount">dayCount</b>
		 - Type: `integer`
		 - Default: `1`
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/tableJoins/properties/columnJoins">columnJoins</b>
		 - Type: `array`
			 - **Items**
			 - &#36;ref: [#/definitions/columnJoins](#/definitions/columnJoins)


**tableData**

 - Type: `object`
 - This schema <u>does not</u> accept additional properties.
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/tableData/properties/columns">columns</b>
		 - Type: `array`
			 - **Items**
			 - &#36;ref: [#/definitions/columnName](#/definitions/columnName)
	 - <b id="#https://open-metadata.org/schema/entity/data/table.json/definitions/tableData/properties/rows">rows</b>
		 - Type: `array`
			 - **Items**
			 - Type: `array`
				 - **Items**
				 - Type: `string`
			 - 
				 - Type: `number`
			 - 


