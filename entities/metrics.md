# Metrics

This schema defines the Metrics entity. Metrics are measurements computed from data such as `Monthly Active Users`. Some of the metrics that measures used to determine performance against an objective are called KPIs or Key Performance Indicators, such as `User Retention`.

<b id="https/open-metadata.org/schema/entity/data/metrics.json">&#36;id: https://open-metadata.org/schema/entity/data/metrics.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - Unique identifier that identifies this metrics instance.
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **name** `required`
	 - Name that identifies this metrics instance uniquely.
	 - Type: `string`
	 - Length: between 1 and 64
 - **fullyQualifiedName**
	 - A unique name that identifies a metric in the format 'ServiceName.MetricName'.
	 - Type: `string`
	 - Length: between 1 and 64
 - **description**
	 - Description of metrics instance, what it is, and how to use it.
	 - Type: `string`
 - **href**
	 - Link to the resource corresponding to this entity.
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **owner**
	 - Owner of this metrics.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **service** `required`
	 - Link to service where this metrics is hosted in.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **usageSummary**
	 - Latest usage information for this database.
	 - &#36;ref: [../../type/usageDetails.json](../types/usagedetails.md)
