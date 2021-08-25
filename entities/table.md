# Table

<b id="https/open-metadata.org/schema/entity/data/table.json">&#36;id: https://open-metadata.org/schema/entity/data/table.json </b>

Type: `object`

## Properties
### id `required`
 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
### name `required`
 - &#36;ref: [#/definitions/tableName](#tablename)
### description
Type: `string`

### href
 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
### tableType
 - &#36;ref: [#/definitions/tableType](#tabletype)
### fullyQualifiedName
Type: `string`

### columns `required`
Type: `array`

### Items
&#36;ref: [#/definitions/column](#column)

### tableConstraints
Type: `array`

### Items
&#36;ref: [#/definitions/tableConstraint](#tableconstraint)

### usageSummary
 - &#36;ref: [../../type/usageDetails.json](../types/usagedetails.md)
### owner
 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
### followers
 - &#36;ref: [../../type/entityReference.json#/definitions/entityReferenceList](../types/entityreference.md#entityreferencelist)
### database
 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
### viewDefinition
 - &#36;ref: [../../type/basic.json#/definitions/sqlQuery](../types/basic.md#sqlquery)
### tags
Type: `array`

### Items
&#36;ref: [../../type/tagLabel.json](../types/taglabel.md)

### joins
 - &#36;ref: [#/definitions/tableJoins](#tablejoins)
### sampleData
 - &#36;ref: [#/definitions/tableData](#tabledata)


## Type definitions in this schema
### tableType

Type: `string`

 - The value is restricted to the following: 
	 1. _"Regular"_
	 2. _"External"_
	 3. _"View"_
	 4. _"SecureView"_
	 5. _"MaterializedView"_


### columnDataType

Type: `string`

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


### columnConstraint

Type: `string`

 - The value is restricted to the following: 
	 1. _"NULL"_
	 2. _"NOT_NULL"_
	 3. _"UNIQUE"_
	 4. _"PRIMARY_KEY"_
 - Default: _"NULL"_


### tableConstraint

Type: `object`

### Properties
 - ### constraintType
 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"UNIQUE"_
		 2. _"PRIMARY_KEY"_
		 3. _"FOREIGN_KEY"_
 - ### columns
 - Type: `array`
### Items
Type: `string`



### columnName

Type: `string`

 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


### tableName

Type: `string`

 - The value must match this pattern: `^[^.]*$`
 - Length: between 1 and 64


### fullyQualifiedColumnName

Type: `string`

 - Length: between 1 and 256


### column

Type: `object`

### Properties
 - ### name `required`
	 - &#36;ref: [#/definitions/columnName](#columnname)
 - ### columnDataType `required`
	 - &#36;ref: [#/definitions/columnDataType](#columndatatype)
 - ### description
 - Type: `string`
 - ### fullyQualifiedName
	 - &#36;ref: [#/definitions/fullyQualifiedColumnName](#fullyqualifiedcolumnname)
 - ### tags
 - Type: `array`
### Items
 - &#36;ref: [../../type/tagLabel.json](../types/taglabel.md)
 - ### columnConstraint
	 - &#36;ref: [#/definitions/columnConstraint](#columnconstraint)
 - ### ordinalPosition
 - Type: `integer`


### columnJoins

Type: `object`

 - This schema <u>does not</u> accept additional properties.
### Properties
 - ### columnName
	 - &#36;ref: [#/definitions/columnName](#columnname)
 - ### joinedWith
 - Type: `array`
### Items
Type: `object`

### Properties
 - ### fullyQualifiedName
	 - &#36;ref: [#/definitions/fullyQualifiedColumnName](#fullyqualifiedcolumnname)
 - ### joinCount
 - Type: `integer`


### tableJoins

Type: `object`

 - This schema <u>does not</u> accept additional properties.
### Properties
 - ### startDate
	 - &#36;ref: [../../type/basic.json#/definitions/date](../types/basic.md#date)
 - ### dayCount
 - Type: `integer`
	 - Default: `1`
 - ### columnJoins
 - Type: `array`
### Items
 - &#36;ref: [#/definitions/columnJoins](#columnjoins)


### tableData

Type: `object`

 - This schema <u>does not</u> accept additional properties.
### Properties
 - ### columns
 - Type: `array`
### Items
 - &#36;ref: [#/definitions/columnName](#columnname)
 - ### rows
 - Type: `array`
### Items
Type: `array`

### Items
 - Type: `string`
 - 
 - Type: `number`
 - 


