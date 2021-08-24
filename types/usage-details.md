# Type used to return usage details of an entity

<b id="httpsopen-metadata.orgschematypeusagedetails.json">&#36;id: https://open-metadata.org/schema/type/usageDetails.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/type/usageDetails.json/properties/dailyStats">dailyStats</b> `required`
	 - &#36;ref: [#/definitions/usageStats](#/definitions/usageStats)
 - <b id="#https://open-metadata.org/schema/type/usageDetails.json/properties/weeklyStats">weeklyStats</b>
	 - &#36;ref: [#/definitions/usageStats](#/definitions/usageStats)
 - <b id="#https://open-metadata.org/schema/type/usageDetails.json/properties/monthlyStats">monthlyStats</b>
	 - &#36;ref: [#/definitions/usageStats](#/definitions/usageStats)
 - <b id="#https://open-metadata.org/schema/type/usageDetails.json/properties/date">date</b> `required`
	 - &#36;ref: [basic.json#/definitions/date](#basic.jsondefinitionsdate)


## Type definitions in this schema
**usageStats**

 - Type: `object`
 - This schema <u>does not</u> accept additional properties.
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/type/usageDetails.json/definitions/usageStats/properties/count">count</b> `required`
		 - Type: `integer`
		 - Range:  &ge; 0
	 - <b id="#https://open-metadata.org/schema/type/usageDetails.json/definitions/usageStats/properties/percentileRank">percentileRank</b>
		 - Type: `number`
		 - Range: between 0 and 100


