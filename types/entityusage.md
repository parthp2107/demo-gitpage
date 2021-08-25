# Usage details of an entity

This schema defines the type used for capturing usage details of an entity.

<b id="https/open-metadata.org/schema/type/entityusage.json">&#36;id: https://open-metadata.org/schema/type/entityUsage.json</b>

Type: `object`

## Properties
 - **entity** `required`
	 - Entity for which usage is returned.
	 - &#36;ref: [entityReference.json](entityreference.md)
 - **usage** `required`
	 - List usage details per day.
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [usageDetails.json](usagedetails.md)
