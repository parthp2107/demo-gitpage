# Thread

<b id="httpsopen-metadata.orgschemaentityfeedthread.json">&#36;id: https://open-metadata.org/schema/entity/feed/thread.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)
 - **href**
	 - &#36;ref: [../../type/basic.json#/definitions/href](....typebasic.mddefinitionshref)
 - **threadTs**
	 - &#36;ref: [../../type/basic.json#/definitions/dateTime](....typebasic.mddefinitionsdatetime)
 - **about** `required`
	 - &#36;ref: [../../type/basic.json#/definitions/entityLink](....typebasic.mddefinitionsentitylink)
 - **addressedTo**
	 - &#36;ref: [../../type/basic.json#/definitions/entityLink](....typebasic.mddefinitionsentitylink)
 - **posts** `required`
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/post](definitionspost)


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
		 - &#36;ref: [../../type/basic.json#/definitions/uuid](....typebasic.mddefinitionsuuid)


