# Basic

<b id="httpsopen-metadata.orgschematypebasic.json">&#36;id: https://open-metadata.org/schema/type/basic.json</b>



## Type definitions in this schema
**uuid**

 - Type: `string`
 - String format must be a "uuid"


**email**

 - Type: `string`
 - String format must be a "email"
 - The value must match this pattern: `^\S+@\S+\.\S+$`
 - Length: between 6 and 127


**entityLink**

 - Type: `string`
 - The value must match this pattern: `^<#E/\S+/\S+>$`


**timestamp**

 - Type: `string`
 - String format must be a "utc-millisec"


**href**

 - Type: `string`
 - String format must be a "uri"


**timeInterval**

 - Type: `object`
 - **Properties**
	 - <b id="#https://open-metadata.org/schema/type/basic.json/definitions/timeInterval/properties/start">start</b>
		 - Type: `integer`
	 - <b id="#https://open-metadata.org/schema/type/basic.json/definitions/timeInterval/properties/end">end</b>
		 - Type: `integer`


**duration**

 - Type: `string`


**date**

 - Type: `string`
 - String format must be a "date"


**dateTime**

 - Type: `string`
 - String format must be a "date-time"


**sqlQuery**

 - Type: `string`


