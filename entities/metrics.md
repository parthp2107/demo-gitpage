# Metrics

<b id="https/open-metadata.org/schema/entity/data/metrics.json">&#36;id: https://open-metadata.org/schema/entity/data/metrics.json </b>

Type: `object`

## Properties
### id `required`
 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
### name `required`
Type: `string`

 - Length: between 1 and 64
### fullyQualifiedName
Type: `string`

 - Length: between 1 and 64
### description
Type: `string`

### href
 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
### owner
 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
### service `required`
 - &#36;ref: [../../type/entityReference.json](../types/entityreference.md)
### usageSummary
 - &#36;ref: [../../type/usageDetails.json](../types/usagedetails.md)
