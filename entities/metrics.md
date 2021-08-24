# Metrics

<b id="httpsopen-metadata.orgschemaentitydatametrics.json">&#36;id: https://open-metadata.org/schema/entity/data/metrics.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/name">name</b> `required`
	 - Type: `string`
	 - Length: between 1 and 64
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/fullyQualifiedName">fullyQualifiedName</b>
	 - Type: `string`
	 - Length: between 1 and 64
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/description">description</b>
	 - Type: `string`
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/href">href</b>
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/owner">owner</b>
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/service">service</b> `required`
	 - &#36;ref: [../../type/entityReference.json](#....typeentityreference.json)
 - <b id="#https://open-metadata.org/schema/entity/data/metrics.json/properties/usageSummary">usageSummary</b>
	 - &#36;ref: [../../type/usageDetails.json](#....typeusagedetails.json)
