# Profile

This schema defines the type for a profile of a user, team, or organization.

<b id="https/open-metadata.org/schema/type/profile.json">&#36;id: https://open-metadata.org/schema/type/profile.json</b>

Type: `object`

## Properties
 - **images**
	 - $ref: [#/definitions/imageList](#imagelist)


## Type definitions in this schema
### imageList

 - Links to a list of images of varying resolutions/sizes.
 - Type: `object`
 - **Properties**
	 - **image**
		 - Type: `string`
		 - String format must be a "uri"
	 - **image24**
		 - Type: `string`
		 - String format must be a "uri"
	 - **image32**
		 - Type: `string`
		 - String format must be a "uri"
	 - **image48**
		 - Type: `string`
		 - String format must be a "uri"
	 - **image72**
		 - Type: `string`
		 - String format must be a "uri"
	 - **image192**
		 - Type: `string`
		 - String format must be a "uri"
	 - **image512**
		 - Type: `string`
		 - String format must be a "uri"


