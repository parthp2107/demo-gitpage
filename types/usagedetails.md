# Type used to return usage details of an entity

<b id="httpsopen-metadata.orgschematypeusagedetails.json">&#36;id: https://open-metadata.org/schema/type/usageDetails.json</b>

Type: `object`

## Properties
 - **dailyStats** `required`
	 - &#36;ref: [#/definitions/usageStats](definitionsusagestats)
 - **weeklyStats**
	 - &#36;ref: [#/definitions/usageStats](definitionsusagestats)
 - **monthlyStats**
	 - &#36;ref: [#/definitions/usageStats](definitionsusagestats)
 - **date** `required`
	 - &#36;ref: [basic.json#/definitions/date](basic.mddefinitionsdate)


## Type definitions in this schema
### usageStats

 - Type: `object`
 - This schema <u>does not</u> accept additional properties.
 - **Properties**
	 - **count** `required`
		 - Type: `integer`
		 - Range:  &ge; 0
	 - **percentileRank**
		 - Type: `number`
		 - Range: between 0 and 100


