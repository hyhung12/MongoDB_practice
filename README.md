# MongoDB_practice
- Connect
```
mongos "mongodb+srv://cluster0.ijfrnwn.mongodb.net/myFirstDatabase" --apiVersion 1 --username hyhung12
```
- Query
```
db.restaurants.find({}, name:1, borough:1, _id:0, "address.zipcode:1"}
db.restaurants.find({'borough':'Bronx'}).limit(5)
db.restaurants.find({'borough':'Bronx'}).skip(2).limit(5)
```
- Distinct
```
db.restaurants.distinct('borough')
