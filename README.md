## MongoDB-Exercise-02

**1. Create a Database called customers.**
```
use customers
switched to db customers
```
**2. Create a collection called customerdetails.**
```
db.createCollection("customerdetails")
```
**3. Insert all documents into the collection named   customerdetails.**
```
customers> db.customerdetails.insertMany([{ "name":"John","age":"25","gender":"Male","city":"New york"},{"name":"Emily","age":"22","gender":"Female","city":"London"},{"name":"Daniel","age":"28","gender":"Male","city":"Sydney"},{"name":"Sophia","age":"24","gender":"Female","city":"Paris"},{"name":"William ","age":"26","gender":"Male","city":"Chicago"},{"name":"Olivia","age":"23","gender":"Female","city":"Los Angeles"},{"name":"Benjamin","age":"27","gender":"male","city":"Toronto"},{"name":"Mila","age":"29","gender":"Female","city":"Berlin"},{"name":"James","age":"30","gender":"Male","city":"Tokyo"}])

```
**4. Retrieve all documents from the collection and sort the results by the “age” field    in ascending order.**

```
customers> db.customerdetails.find().sort({ age: 1 }).pretty()
[
  {
    _id: ObjectId("654caf087b527d586e7f2e1d"),
    name: 'Emily',
    age: '22',
    gender: 'Female',
    city: 'London'
  },

  {
    _id: ObjectId("654cb4b87b527d586e7f2e24"),
    name: 'Olivia',
    age: '23',
    gender: 'Female',
    city: 'Los Angeles'
  },
  {
    _id: ObjectId("654cb4b87b527d586e7f2e22"),
    name: 'Sophia',
    age: '24',
    gender: 'Female',
    city: 'Paris'
  },
  {
    _id: ObjectId("654caf087b527d586e7f2e1c"),
    name: 'John',
    age: '25',
    gender: 'Male',
    city: 'New york'
  },
  {
    _id: ObjectId("654cb4b87b527d586e7f2e1f"),
    name: 'John',
    age: '25',
    gender: 'Male',
    city: 'New york'
  },
  {
    _id: ObjectId("654cb4b87b527d586e7f2e23"),
    name: 'William ',
    age: '26',
    gender: 'Male',
    city: 'Chicago'
  },
  {
    _id: ObjectId("654cb4b87b527d586e7f2e25"),
    name: 'Benjamin',
    age: '27',
    gender: 'male',
    city: 'Toronto'
  },
  {
    _id: ObjectId("654caf087b527d586e7f2e1e"),
    name: 'Daniel',
    age: '28',
    gender: 'Male',
    city: 'Sydney'
  },

  {
    _id: ObjectId("654cb4b87b527d586e7f2e26"),
    name: 'Mila',
    age: '29',
    gender: 'Female',
    city: 'Berlin'
  },
  {
    _id: ObjectId("654cb4b87b527d586e7f2e27"),
    name: 'James',
    age: '30',
    gender: 'Male',
    city: 'Tokyo'
  }
]

```
**5.Count the number of females.**
```
customers> db.customerdetails.countDocuments({"gender":"Female"})
5
```
**6.Insert one document into the customerdetails collection.**
```
customers> db.customerdetails.insertOne({"name":"Dilani","age":"23","gender":"Female","city":"Jaffna"})
{
  acknowledged: true,
  insertedId: ObjectId("654d24bfaf44c2506fe4219a")
}
```
**7. Update city=SriLanka to John.**
```

```
**8. Remove the customer from Tokyo.**
```
```

**9.  Find customers not from Los Angeles.**
```
```

**10.Find the customers who are older than age 25.**
```
```

**11.Retrieve the males who are less than 25.**
```
```

**12.Update Francis age to 35, if Francis is not available upsert.**
```
```
**13.Retrieve males who are younger than 30 and older than25.**
```

```

**14.Find a customer who is lesser than or equal to 23.**
```
```
**15.Remove the customer from Tokyo.**
```
```


