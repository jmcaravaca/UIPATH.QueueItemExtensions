# UIPath Queue Item extensions

## Queue Item Activities
This library provides a number of additional methods to handle UIPath Queue Items for common tasks. The activities integrate directly into a process using the standard robot execution permissions and standard UIPath Variables

The methods currently included are:
- Get All Queue Items: This activity bypasses the "100" limit on the standard "Get Queue Items" activity, expanding that limit to 10.000
- Get Queue Retries: Returns the preconfigured "number of retries" of an Orchestrator Queue
- Get QueueItem Processing Times: Returns the Start, End, and total number of seconds spent doing a QueueItem
- Get Queue Items By Specific Data: Returns queue items using a key-value pair to filter in the "SpecificContent" of a Queue Item
- Get Queue ITems By Progress: Returns queue items filtering by the "Progress" field

## How it works
All the activities make use of the Orchestrator API to retrieve data, applying the necessary transformations to return the values as either QueueItems or primitive variables


## Dependencies and versions

These activities have been tested with UiPath Studio 21.10.6, using Orchestrator 22.4.1