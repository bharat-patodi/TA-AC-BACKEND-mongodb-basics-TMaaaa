writeCode

Write code to:-

- create a database named `sports`.
<!-- use sports -->
- list all databases present in local mongod server.
<!-- show dbs -->
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
<!--
db.createCollection("cricket")
db.createCollection("football")
db.createCollection("TT")
-->
- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
<!--
 db.khokho.insert([{name: "giri", age: "12", email: "giri@gmail.com", bid_price: "12000"}, {name: "goru", age: "14", email: "name@goru.com", bid_price: "13999"}, {name: "hide", age: "45", email: "hide@goru.com", bid_price: "160000"}])

db.football.insert([{name: "hitesh", age: "32", email: "hitesh@gmail.com", bid_price: "100000"}, {name: "fatima", age: "43", email: "name@fatima.com", bid_price: "19999"}, {name: "clyde", age: "45", email: "clyde@goru.com", bid_price: "100"}])

db.TT.insert([{name: "tahir", age: "21", email: "tahir@gmail.com", bid_price: "1000"}, {name: "ttlover", age: "4", email: "name@ttlover.com", bid_price: "1"}, {name: "sunil", age: "5", email: "sunil@name.com", bid_price: "1000000"}])

-->

- list all collections in sports database.
<!-- show collections -->
- rename `TT` collection to `tennis`.
<!-- db.TT.renameCollection("tennis") -->
- create a capped collection called `khokho` which should have max 3 documents.
  <!-- db.createCollection("khokho", {capped: true, size: 10000, max: 3}) -->
  Try inserting more than 3 and see what happens?
  <!-- The new entry overwrites the first entry -->
- check whether a collection is capped or not?
<!-- db.khokho.isCapped() -->
- drop all documents from `football` collection.
<!-- db.football.remove({}) -->
- delete cricket collection completely.
<!-- db.cricket.drop() -->
- delete sports database.
<!-- db.dropDatabase() -->
- check which database you are connected to ?
<!-- sports -->
- connect to test database
<!-- use test -->
