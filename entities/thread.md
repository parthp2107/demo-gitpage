# Thread

This schema defines the Thread entity. A Thread is a collection of posts made by the users. The first post that starts a thread is **about** a data asset **from** a user. Other users can respond to this post by creating new posts in the thread. Note that bot users can also interact with a thread. A post can contains links that mention Users or other Data Assets.

<b id="https/open-metadata.org/schema/entity/feed/thread.json">&#36;id: https://open-metadata.org/schema/entity/feed/thread.json</b>

Type: `object`

## Properties
 - **id** `required`
	 - Unique identifier that identifies an entity instance.
	 - $ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)
 - **href**
	 - Link to the resource corresponding to this entity.
	 - $ref: [../../type/basic.json#/definitions/href](../types/basic.md#href)
 - **threadTs**
	 - Timestamp of the when the first post created the thread.
	 - $ref: [../../type/basic.json#/definitions/dateTime](../types/basic.md#datetime)
 - **about** `required`
	 - Data asset about which this thread is created for with format <#E/{enties}/{entityName}/{field}/{fieldValue}.
	 - $ref: [../../type/basic.json#/definitions/entityLink](../types/basic.md#entitylink)
 - **addressedTo**
	 - User or team this thread is addressed to in format <#E/{enties}/{entityName}/{field}/{fieldValue}.
	 - $ref: [../../type/basic.json#/definitions/entityLink](../types/basic.md#entitylink)
 - **posts** `required`
	 - Type: `array`
		 - **Items**
		 - $ref: [#/definitions/post](#post)


## Type definitions in this schema
### post

 - Post within a feed.
 - Type: `object`
 - **Properties**
	 - **message** `required`
		 - Message in markdown format. See markdown support for more details.
		 - Type: `string`
	 - **postTs**
		 - Timestamp of the post.
		 - Type: `string`
		 - String format must be a "date-time"
	 - **from** `required`
		 - ID of User (regular user or a bot) posting the message.
		 - $ref: [../../type/basic.json#/definitions/uuid](../types/basic.md#uuid)



This Document was generated on: Thursday, August 26, 2021