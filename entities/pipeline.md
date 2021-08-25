# Pipeline

<b id="httpsopen-metadata.orgschemaentitydatapipeline.json">&#36;id: https://open-metadata.org/schema/entity/data/pipeline.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)
 - **name** `required`
	 - Type: `string`
	 - Length: between 1 and 64
 - **fullyQualifiedName**
	 - Type: `string`
	 - Length: between 1 and 64
 - **description**
	 - Type: `string`
 - **href**
	 - &#36;ref: [../../type/basic.json#/definitions/href](....typebasic.mddefinitionshref)
 - **owner**
	 - &#36;ref: [../../type/entityReference.json](....typeentityreference.md)
 - **service** `required`
	 - &#36;ref: [../../type/entityReference.json](....typeentityreference.md)
