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

2. dashboard Thake Create a cluster akta new cluster add kore nite hobe 
3.  free ta select kore nobo and name rakhe dibo cluster0 and je kno akta cuntry selet kore nibo and AWS selet kore nobo . 
4. user name and pasword amra copy kore rakhbo pore kaj a lagbe  user name: sdsofik2002_db_user pasword: vxTstZitGwjiSK8w tarpor closd kore dibo .
5. আমরা তারপর mongos Compass a connet korbo?  আমরা Connect clik korbo kore user name and password দিয়ে craate Databas user clik kore nibo  click করার por chose to connction method a clik korbo সাথে সাথে  সব গুলা connet option চলে আসবে drive vs code and commpass আমরা যেহেতু commpass a conncet krobo tao commpass select kore nibo 

তারপর নিছে একটা লিঙ্কস পাবো ওইটা কপি করে নিব নিয়ে চলে জাব commpass a 

6. তারপর আমরা একটা নতুন crate করে নিব url oi links ta dibo user name জায়গায় ইউজার নামে থাকবে password er jaygay oi pasword ta dibo তারপর একটা ইউজার নামে দিয়ে অ্যান্ড একটা color select kore নিয়ে save and change kore nibo যদি সব কিছু ঠিক থাকে থলে ওকে না হলে error দিবে 

7. atlas a গিয়ে network access গিয়ে IP Access List a edit a giye all acees diye dibo all ip 
8. আমরা atlas a kaj korbo na কারন অনেক স্লও থাকে তাই আমরা commpass a kaj korbo 
9. new data bas create kore nita parbo 

/// ================Database Related Method ===================

mongodb commet 

আমরা commpres a giye কেন একটা click করে Open mongoBD shell select kore commed dibo 

>use দিয়ে কন ডাটাবেস জাবো তা সিলেক্ট করে নিতে পারব ।
> cls দিয়ে আমরা despily clean kore নিতে পারব 
> db.getName() দিয়ে আমরা কোন ফাইল বা ডাটাবেস  এ আছি ওই ডাটাবেস তা দেখতে পারব । 
>db.stata() দিয়ে আমরা ডাটাবেসর সকল statas দেখতে পাব 
> db.collectionName() দিয়ে আমরা যে ডাটাবেস  এ আছি ওইখানের সব collection দেখতে পারব ।
>db.createCollection("collection name") দিয়ে আমরা নেউ collection বানাইতে পারব ।
>db.getMongo() দিয়ে আমরা ওই mongodb connect string টা পাবো ।
> db.dropDatabas() যদি দেই আমরা তাহলে আমদের ওই ডাটাবেস টা ডিলিট হয়ে যাবে একবার ।
>db.serverStats() দিয়ে database server all infofromtion পাওয়া যায় ।
>db.hostInfo () দিয়ে database er CPU OS and hardware all info দেখা যায় 
>db.getProfilingStats() দিয়ে আমদের database এ কেনো লান্দি প্রসেস আছে নাকি তা দেখায় ।
>db.correntOp() দিলে আমদের কি কি অপারেশান চলে তা সব দেখাবে 
>show dbs দিলে আমদের যে যে databas আছে সব দেখতে পাই ।
>use diye data file er name creare kore nibo collection.

=================  collections drop and create =============================

collections হল যেখানে dataBase সকল ডাটা জমা থাকে 




