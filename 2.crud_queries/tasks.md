1. Create a database named `blog`.

<!-- use blog -->

2. Create a collection called 'articles'.

<!-- db.createCollection('articles') -->

3. Insert multiple documents(at least 3) into articles. It should have fields

<!-- db.articles.insertMany([{title:'human',name:'sunny',details:'null'},{title:'human',name:'bunny',details:'null'},{title:'human',name:'honey',details:'null'}]) -->


4. Find all the articles using `db.COLLECTION_NAME.find()`

<!-- db.articles.find() -->

5. Find a document using _id field.

<!-- db.articles.find({_id:ObjectId("5d9f5daff916f7ccd55562cc")}) -->

6. Find documents using title and author's name field.

<!-- db.articles.find({'title':'human','name':'sunny'}); -->


7. Find document using a specific tag.

<!-- db.articles.find({},{title:1}); -->
<!-- db.articles.find({},{name:1) -->

8. Update title of a document using its _id field.

<!-- db.article.update({_id:ObjectId("5d9f5daff916f7ccd55562cc"),{$set:{title:'animal'}}}) -->

9. Update a author's name using article's title.

<!-- db.articles.update({title:"human"},{$set:{name:'rocky'}}); -->

10. rename details field to description from articles collection.

<!-- db.articles.rename({'details','description'}) -->

11. Add additional tag in a specific document.

<!-- db.articles.update({_id:ObjectId("5d9f5ed5f916f7ccd55562d0")},{$set:{tag:{address:"delhi"}}}); -->

12. Update an article's tags using $set and without $set.
  - Write the differences here ?

  <!-- db.articles.update({_id:ObjectId("5d9f5ed5f916f7ccd55562d0")},{$set:{tags:{"location":"dharamshala"}}}) -->
  only add additional datas to the collection without removing old datas.
  <!-- db.articles.update({_id:ObjectId("5d9f5ed5f916f7ccd55562d0")},{tags:{"location":"dharamshala"}}}) -->
  replaces old datas and add new datas.

13. Increment an auhtor's age by 5.  



14. Delete a document using _id field with `db.COLLECTION_NAME.remove()`.
<!-- db.articles.remove({id:ObjectId("5d9f5ed5f916f7ccd55562d0")},{}) -->

Use sample.js data for below queries.

1. Find all males who play cricket.

2. Update user with extra golf field in sports array whose name is "Steve Ortega".

3. Find all users who play either 'football' or 'cricket'.

4. Find all users whose name includes 'ri' in their name.
