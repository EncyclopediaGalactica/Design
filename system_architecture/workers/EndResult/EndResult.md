# EndResult Worker specification

EndResult worker is always the last point in any given operation as the end result of a process
lands here for later publishing. A slot has to be created for publishing, and requesting 
the slot should happen early in the process.

EndResult Worker sends event data to EventJournal.

In order to avoid dead content in the database a periodic job will be run to clean up 
content already exceeded its lifetime.

## Api

### Create
Creating a slot where to the result can be pushed. The content is always a serialized 
object.
#### Parameters

- Lifetime in seconds

### Get
It returns the content of a slot.
#### Parameters
- Id of the slot which is a GUID.

### Delete
Deletes the slot.
#### Parameters
- Id of the slot which is a GUID.

## Simplified database schema

|Column name|Type|Description|
|---|---|---|
|id|GUID|Unique Identifier|
|content|TEXT|The serialized content|
|created_at|Datetime|Date of creation|
|lifetime|INT|Slot lifetime in seconds|

## Technical details

- The worker is implemented by .NET 5 Generic Host.
- Database is PostgreSQL
- container is Docker and running on Kubernetes

## Future possibilities

- the database can be changed to Redis to achieve higher throughput
