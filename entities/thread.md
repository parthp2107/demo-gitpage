# Thread

<b id="httpsopen-metadata.orgschemaentityfeedthread.json">&#36;id: https://open-metadata.org/schema/entity/feed/thread.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/properties/id">id</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)
 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/properties/href">href</b>
	 - &#36;ref: [../../type/basic.json#/definitions/href](#....typebasic.jsondefinitionshref)
 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/properties/threadTs">threadTs</b>
	 - &#36;ref: [../../type/basic.json#/definitions/dateTime](#....typebasic.jsondefinitionsdatetime)
 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/properties/about">about</b> `required`
	 - &#36;ref: [../../type/basic.json#/definitions/entityLink](#....typebasic.jsondefinitionsentitylink)
 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/properties/addressedTo">addressedTo</b>
	 - &#36;ref: [../../type/basic.json#/definitions/entityLink](#....typebasic.jsondefinitionsentitylink)
 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/properties/posts">posts</b> `required`
	 - Type: `array`
		 - **Items**
		 - &#36;ref: [#/definitions/post](#/definitions/post)


## Type definitions in this schema
**post**

 - Type: `object`
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/definitions/post/properties/message">message</b> `required`
		 - Type: `string`
	 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/definitions/post/properties/postTs">postTs</b>
		 - Type: `string`
		 - String format must be a "date-time"
	 - <b id="#https://open-metadata.org/schema/entity/feed/thread.json/definitions/post/properties/from">from</b> `required`
		 - &#36;ref: [../../type/basic.json#/definitions/uuid](#....typebasic.jsondefinitionsuuid)


