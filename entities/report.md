# Report

This schema defines the Report entity. Reports are static information computed from data periodically that includes data in text, table, and visual form.

<b id="https/open-metadata.org/schema/entity/data/report.json">&#36;id: https://open-metadata.org/schema/entity/data/report.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - Unique identifier that identifies this report.
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **name** `required`
	 - Name that identifies this report instance uniquely.
	 - Type: `string`
	 - Length: between 1 and 64
 - **fullyQualifiedName**
	 - A unique name that identifies a report in the format 'ServiceName.ReportName'.
	 - Type: `string`
	 - Length: between 1 and 64
 - **description**
	 - Description of this report instance.
	 - Type: `string`
 - **href**
	 - Link to the resource corresponding to this report.
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **owner**
	 - Owner of this pipeline.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **service** `required`
	 - Link to service where this report is hosted in.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **usageSummary**
	 - Latest usage information for this database.
	 - &#36;ref: [../../type/usageDetails.json](../types/usagedetails.md)
