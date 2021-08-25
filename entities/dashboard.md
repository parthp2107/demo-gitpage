# Dashboard

This schema defines the Dashboard entity. Dashboards are computed from data and visually present data, metrics, and KPIs. They are updated in real-time and allow interactive data exploration.

<b id="https/open-metadata.org/schema/entity/data/dashboard.json">&#36;id: https://open-metadata.org/schema/entity/data/dashboard.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - Unique identifier that identifies a dashboard instance.
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **name** `required`
	 - Name that identifies this dashboard.
	 - Type: `string`
	 - Length: between 1 and 64
 - **fullyQualifiedName**
	 - A unique name that identifies a dashboard in the format 'ServiceName.DashboardName'.
	 - Type: `string`
	 - Length: between 1 and 64
 - **description**
	 - Description of the dashboard, what it is, and how to use it.
	 - Type: `string`
 - **href**
	 - Link to the resource corresponding to this entity.
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **owner**
	 - Owner of this dashboard.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **service** `required`
	 - Link to service where this dashboard is hosted in.
	 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
 - **usageSummary**
	 - Latest usage information for this database.
	 - &#36;ref: [../../type/usageDetails.json](../types/usagedetails.md)
