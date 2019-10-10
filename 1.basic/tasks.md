#### write commands for following mongodb opertaions

1. create a database named `sports`
// Answer here ..

<!-- use sports -->

2. list all databases present in local mongod server.
// Answer here..

<!-- show dbs -->


3. create 3 collections named `cricket`, `football`, `TT` in sports database.

<!-- db.createCollection(`cricket`) -->
<!-- db.createCollection(`football`) -->
<!-- db.createCollection(`TT`) -->


4. add 3 players in each of above collections which should have fields like `name`, `age`, `email`, state and auction_price.


<!-- db.cricket.insert({name:'sunny',age:'21',email:'sunny@mac'}) -->
<!-- db.football.insert({name:'sunny',age:'21',email:'sunny@mac'}) -->
<!-- db.TT.insert({name:'sunny',age:'21',email:'sunny@mac'}) -->


5. list all collections in sports database.


<!-- show collections -->
<!-- cricket -->
<!-- football -->
<!-- TT -->


6. rename `TT` collection to `tennis`.


<!-- db.renameCollection(`TT`,`tennis`) -->


7. create a capped collection called `khokho` which should have max 3 documents.
  Try inserting more than 3 and output the result here ?


<!-- db.createCollection(`khokho`,{ capped:true ,size:1024, max:3 }) -->


8. check whether a collection is capped or not?


<!-- db.khokho.isCapped() -->


9. remove all documents from `football` collection.


<!-- db.football.remove({}) -->


10. delete cricket collection completely.


<!-- db.cricket.drop() -->


11. rename database sports to games

<!-- db.renameCollection(sports,games) -->

12. delete sports database. 

<!-- db.dropDatabase() -->