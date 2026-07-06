what is a MongoDB ?

Answer: MongoDB হলো একটি Non SQL DataBase যেখানে data Documents আকারে সংরক্ষণ করা হয় ।
এটি traditional SQL database (যেমন MySQL, PostgreSQL) এর মতো table, row, column ব্যবহার না করে collections এবং documents ব্যবহার করে।

| SQL Database | MongoDB    |
| ------------ | ---------- |
| Database     | Database   |
| Table        | Collection |
| Row          | Document   |
| Column       | Field      |


উদাহরণ SQL-এ: 

ID | Name | Age
1  | Rahim | 25
2  | Karim | 30

MongoDB-তে:

{
  "_id": 1,
  "name": "Rahim",
  "age": 25
}

MOngoDB data সব সময় json Formet a thake 

why use MongoDB ?

1. Flexible structure   এইটা sql এর মত টেবিল লাগে না 
2. Rapid scale-up and scale-out   হাজার হাজার ডাটা এক সাথে hid করলেও আমরা server diye handle kortce pari 

3. Direct match to JSON  
4. start-up friendly 


MongoBD server Setup 

1. Mongodb Community server 
হল যেটা local pc server হয় সকল ডাটা pc জমা থাকে 
2. MongoDB Atlas  যেটা cloud server a জমা থাকে 

mogondb community server Setup 
1. https://www.mongodb.com/try/download/community  এই লিঙ্কস এ গিয়ে পিসির configaration দেখে dowloand kore nite hbe 
2. next and arrger 
3. compelet a jabo tarpor next 
4. setup করার সময় mongodb compass টিক মার্ক দিব

শেষ এ চেক করে নিব mongodb and mongodb compass install hoice ki na 


================ Compass GUI ===========================

add new তে click করব এবং নামে local ba onno kisu dibo je kno akta color select kore nibo 

যদি কখনো না হয় তাহলে কি করব url a  mongodb://localhost:27017  যেটা আছে ওইখানে localhost remove kore 127.0.0.1:  aita diye dibo 

defult a kisu দেওয়া থাকবে আমরা চাইলে আরো অ্যাড করে পারি  + এ ক্লিক করে নিউ নামে দিয়ে করে নিতে পারি ।


====================== Connect Atlas system ==========================

1. (https://www.mongodb.com/) ai urla গিয়ে একটা অ্যাকাউন্ট তৈরি করে নিব email and github ba number diye account kore nibo 

2. dashboard Thake Create a cluster 

