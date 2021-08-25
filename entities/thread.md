# Thread

<b id="https/open-metadata.org/schema/entity/feed/thread.json">&#36;id: https://open-metadata.org/schema/entity/feed/thread.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **href**
	 - &#36;ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **threadTs**
	 - &#36;ref: [../../type/basic.json#/definitions/dateTime](../types/basic.md#datetime)
 - **about** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/entityLink](../types/basic.md#entitylink)
 - **addressedTo**
	 - &#36;ref: [../../type/basic.json#/definitions/entityLink](../types/basic.md#entitylink)
 - **posts** `required`
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/post](#post)


## Type definitions in this schema
### post

 - Type: `object`
 - **Properties**
	 - **message** `required`
		 - Type: `string`
	 - **postTs**
		 - Type: `string`
		 - String format must be a "date-time"
	 - **from** `required`
		 - &#36;ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)


