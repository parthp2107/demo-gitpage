# Tag Label

<b id="https/open-metadata.org/schema/type/taglabel.json">&#36;id: https://open-metadata.org/schema/type/tagLabel.json </b>

Type: `object`

## Properties
 - ### tagFQN
	 - Type: `string`
	 - Length:  &le; 45
 - ### labelType
	 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"Manual"_
		 2. _"Propagated"_
		 3. _"Automated"_
		 4. _"Derived"_
	 - Default: _"Manual"_
 - ### state
	 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"Suggested"_
		 2. _"Confirmed"_
	 - Default: _"Confirmed"_
 - ### href
	 - &#36;ref: [basic.json#/definitions/href](basic.md#href)
