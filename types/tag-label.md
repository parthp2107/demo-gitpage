# Tag Label

<b id="httpsopen-metadata.orgschematypetaglabel.json">&#36;id: https://open-metadata.org/schema/type/tagLabel.json</b>

Type: `object`

## Properties
 - <b id="#https://open-metadata.org/schema/type/tagLabel.json/properties/tagFQN">tagFQN</b>
	 - Type: `string`
	 - Length:  &le; 45
 - <b id="#https://open-metadata.org/schema/type/tagLabel.json/properties/labelType">labelType</b>
	 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"Manual"_
		 2. _"Propagated"_
		 3. _"Automated"_
		 4. _"Derived"_
	 - Default: _"Manual"_
 - <b id="#https://open-metadata.org/schema/type/tagLabel.json/properties/state">state</b>
	 - Type: `string`
	 - The value is restricted to the following: 
		 1. _"Suggested"_
		 2. _"Confirmed"_
	 - Default: _"Confirmed"_
 - <b id="#https://open-metadata.org/schema/type/tagLabel.json/properties/href">href</b>
	 - &#36;ref: [basic.json#/definitions/href](#basic.jsondefinitionshref)
