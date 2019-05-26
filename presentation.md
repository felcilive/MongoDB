`(First horizontal slide)`
We will talk about things like MongoDB in this presentation.
MongoDB is a cross-platform, open-source document database which based on a NoSQL.

`(Second horizontal  slide)`
SQL, unlike Mongo, is a linked table. MongoDB consists of collections. Collection is a group of JSON documents. A document keeps data of key-value.
On this slide you can see other type of document as BSON. BSON is a binary encoding of JSON documents with support for data types which JSON hasn’t got. 

`(Third horizontal slide)`
BSON has the same formats as JSON. But we will talk about new data types right now. 
+ symbol - This datatype is used like a string; but it's generally reserved for languages that use a   specific symbol type.
+ timestamp – This type can be comfortable for recording when a document has been modified.
+ min/max - This type is used to compare a value against the lowest and highest BSON elements.
+ regular expression - This datatype is used to store regular expression.
+ code - This datatype is used to store JavaScript code into the document.
+ binary data - This datatype is used to store binary data.
+ date - This datatype is used to store the current date or time in UNIX time format.
+ object ID - This datatype is used to store the document’s ID.

This is BSON document. Each document must have id. If you do not add id when you create new document, Mongo will generate id itself.
ID - is a 12 bytes hexadecimal number which respond for the uniqueness of every document.


`(Fourth horizontal slide)`
Let’s talk about advantages and disadvantages of MongoDB.
+ fast  - MongoDB is faster and scalabler than SQL server because it uses internal memory for store.
+ horizontal scale – When you work with database you can to get face to face with a trouble, when the current resources of the machine will not be enough for normal operation. Thanks for  horizontal scale, which is easy to use in Mongo, we get infinity machines and better data security.
+ doesn't contain schemas - There is not necessary to create tables, change their schemes, create connections, take care of data types. If you need to change document the only thing that you should to do is to add new line.
+ aggregation - You can use map-reduce, group by difficult conditions, reformat documents in-place and receive random documents.
+ dynamic  - is a deep query-ability. MongoDB supports dynamic requests like powerful as SQL.
+ supports a big amount of data
+ support Agile
+ doesn’t support JOIN and Global transactions


`(Fifth horizontal slide)`
MongoDB has a lot of function for work with database. MongoDB can create, drop, insert, query, update, sort, limit and indexing collections and documents. In this presentation we will not review all methods.  

Function call looks like db.collection_name.command, where
                                          db – is an information about database
                                          
                                          collection_name – is a name of collection
                                          
                                          command -  is a JavaScript-function 

I hope that you will understand simple functions yourself and I will move on to more interesting methods.
+ find()  - is used to query data from collection. 
This method can use such operations as
+ $lt – less than
+ $lte – less than equals
+ $gt – greater than
+ $gte – greater than equals
+ $ne – not equals
+ $and
+ $or
They work like operations in JS.

+ update()/save() – are used to update document into a collection.

But
update() - is used to update the values in the existing document.

save() - is used to replace the existing document with the new document from save() method.

+ limit(number) – is used to limit the records in MongoDB.
Number in brackets means amount of documents which you want to display.
+ sort – is used to sort documents. For sorting takes values 1 and -1. 1 is used for ascending order. -1 is used for descending order.
+ ensureIndex() – is used to create an index. Indexes make searching easy. Without indexes Mongo should scan every document of a collection for searching the request.
+ aggregate() –operations of aggregation process data records and return computed results. This     method has a list of available aggregation expressions ( sum, min, max etc.) And also it has stages in aggregation framework ($project, $match, $group, $sort and etc)

`(Sixth horizontal slide)`
Now we should talk about replication. Replication is a process of synchronizing  data across multiple servers. Replication provides reduces costs and increases data thanks to multiple copies of data on different database servers. Replication protects a database from the lossing of a single server.

Replica set is a group of two or more nodes. In a replica set, one of nodes is primary node and the others nodes are secondary. All data copies from primary to secondary node. If the primary node is disabled, a new primary node will selected. After recovery, the old primary node will work as a secondary.

The next topic which we will consider is a sharding. Sharding is the process of storing data records across multiple machines.

`(Seventh horizontal slide)`
I have told only basic information about MongoDB. Below you can see links of documentation about Mongo and information which I used in this presentation. Thanks for attention.
