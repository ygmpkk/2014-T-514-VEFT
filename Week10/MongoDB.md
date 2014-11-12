#MongoDB

MongoDB is a database that uses a document-oriented data model.  MongoDB does not use tables and rows as relational 
databases do but instead all data is stored in documents and collections.  MongoDB is therefore schema free.   
Data is stored on BSON format which is a binary-encoded serialization of JSON-like documents.  
These objects are added to a collection.  Collections are similar to tables in a relational database. 

MongoDB is a fast and scalable database, it is good for many things but it is not recommended to use this as a database for 
applications that store sensitive data.    

It is easy to run many instances of MongoDB, if that is done the instances replicate the data between them.   

MongoDB does not support traditional sql query language.   Instead it offers its own query language and it is easy 
to find good information about that on the official MongoDB website.

MongoDB is a database server that have to be installed to be used.   

Ubuntu: 
> sudo apt-get install mongodb

The server is started from the command line with the command: mongod.    This command starts up the mongo daemon.

MongoDB needs a data folder and it has to be created with sudo rights:

> sudo mkdir -p /data/db

And then behind closed doors let’s give everyone access rights to this folder:

> chmod –R 777 /data/db

#Mongo

Mongo is a console based client that can be used to query data in MongoDB.  There are also other tools available online 
that have more visual interface such as [Robomongo](http://robomongo.org/)

This command lists all databases
> show database 

This command switches to or creates the database mydb
> use mydb

This command shows all collections in mydb.
> show collections  

To create a collection, create the JSON object 
> var x = {‘user’: ‘hlysig’, ‘course’:’Forritun 1’, ‘grade’:’4’}

To insert into the grades collection give the command:
> db.grades.insert(x)

Further information can be found on [mongoDB](http://www.mongodb.org)

#Mongose

[Mongose](http://mongoosejs.com/) is a framework that can be used in applications to connect to MongoDB.





