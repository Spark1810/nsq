Program1
Create table college(name varchar(20), Rollno varchar(20));
Insert into college (name, Rollno)
Values(“Sailesh”,”21BDS039”);
update college set Rollno= “21BDS060” where name = "Sailesh";

Program2
use college
db.createCollection(“College”)
db.college.insertOne({Name:”Sailesh”,Class:”DS”})

Program3
db.college.insertOne({Name:”Sailesh”,Class:”DS”})
db.college.find({Age: {$gt:20}}).pretty()
db.college.find().pretty()

Program4
db.college.updateOne({Name:”Sailesh”},{$set:{Class:”III DS”}})
db.college.replaceOne({}, {Name:”Someone”,Class”III DS”})

Program5
Export and import the JSON File

Program6
Create a JSON and Import   [{ "Name": "riyan", "Age": 50, "Mark": 450 }, { "Name": "Siruthai", "Age": 15, "Mark": 300 }]

Program7
db.college.createIndex({Name:”text”, Description:”text”})
db.college.find({$text:{$search:"Sailesh"}})

Program8
db.college.find({Name:{$regex:"Sailesh",$options:"i"}})

Program9
Program 3 and Program 4

Program10
Mam responsibility 

Program11
db.college.createIndex({ Name : 1}) 
db.college.createIndex({ Class: 1}) 
db.college.getIndexes()
