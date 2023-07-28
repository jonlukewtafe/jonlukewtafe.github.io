# Databases

---

## MongoDB (NoSQL)

* [How to Design a Document Schema in MongoDB](https://www.digitalocean.com/community/tutorials/how-to-design-a-document-schema-in-mongodb)
* [NoSQL Database Design & Data Modeling (MongoDB)](https://www.mongodb.com/nosql-explained/data-modeling)

## MongoDB Shell URI Components

|URI Component|Meaning|Required/Optional|
|---|---|---|
|mongodb://|Designates this URI as a MongoDB connection|Required unless using mongodb+srv://|
|mongodb+srv://|As above, plus requires a DNS SRV record for the server|Required unless using mongodb://|
|username|The MongoDB username used to access the database|Optional|
|password|The password associated with the MongoDB username used to access the database|Optional|
|host|The host name or IP address|Required|
|port|The host port to use to communicate with the server|Optional (only required if the database being connected to is not using the default port)|
|defaultdb|The default database to access|Optional|

## Various MongoDB Commands

* mongoimport options connection-string file
  * Available Options:
    * /db:DATABASE_NAME - What database should the data be added to?
    * /collection:COLLECTION_NAME - What collection in the database should the data be added to
  * Connection String:
    * /host:IP_ADDRESS OR HOST - Where is the database located? (IP Address or Host)
  * File:
    * FILE_LOCATION/FILE_NAME.FILE_EXTENSION


* [MVVM for Beginners](https://www.codeproject.com/Articles/1112919/MVVM-for-beginners)

{% include_relative footer.md %}
