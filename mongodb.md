<h1> ---------------------- Mongodb Commands---------------------</h1>

---

# 🟢 **1. Start / Connect**

```
mongod                    # Start MongoDB server
mongosh                   # Open MongoDB shell
mongosh "mongodb+srv://<cluster-url>"   # Connect to Atlas
```

---

# 🔵 **2. Database Commands**

```
show dbs                  # List databases
use <dbname>              # Switch / create database
db                        # Show current database
db.dropDatabase()         # Delete current database
```

---

# 🟢 **3. Collection Commands**

```
show collections          # List collections
db.createCollection("name")  
db.<collection>.drop()    # Delete collection
```

---

# 🔶 **4. Insert Commands**

```
db.users.insertOne({name:"A", age:20})
db.users.insertMany([{...}, {...}])
```

---

# 🔷 **5. Read / Find Commands**

```
db.users.find()                 # Show all
db.users.findOne()              # Show one
db.users.find({age:20})         # Filter
db.users.find({age:{$gt:20}})   # age > 20
db.users.find({},{name:1})      # Projection (only name)
db.users.find().sort({age:1})   # Sort
db.users.find().limit(5)        # Limit
db.users.find().count()         # Count
```

---

# 🟣 **6. Update Commands**

```
db.users.updateOne(
  {name:"A"},
  {$set:{age:25}}
)

db.users.updateMany(
  {age:20},
  {$set:{verified:true}}
)
```

Replace entire document:

```
db.users.replaceOne({name:"A"}, {name:"A", age:30})
```

---

# 🔥 **7. Delete Commands**

```
db.users.deleteOne({name:"A"})
db.users.deleteMany({age:20})
```

---

# 🟡 **8. Indexing**

```
db.users.createIndex({name:1})
db.users.createIndex({email:1}, {unique:true})
db.users.getIndexes()
db.users.dropIndex("name_1")
```

---

# 🟠 **9. Aggregation Pipeline**

```
db.users.aggregate([
  {$match:{age:{$gt:20}}},
  {$group:{_id:"$age", total:{$sum:1}}},
  {$sort:{total:-1}}
])
```

Common stages:

```
$match
$group
$sort
$project
$lookup
$limit
$unwind
```

---

# 🔘 **10. User & Authentication**

```
use admin
db.createUser({
  user:"admin",
  pwd:"1234",
  roles:["root"]
})

db.auth("admin", "1234")
```

---

# ⚫ **11. Backup & Restore**

```
mongodump --db=mydb --out=backup/
mongorestore backup/
```

---

# 🟤 **12. Import / Export**

```
mongoimport --db=mydb --collection=users --file=data.json
mongoexport --db=mydb --collection=users --out=users.json
```

---

# 🟣 **13. Server Status / Admin**

```
db.stats()
db.serverStatus()
db.currentOp()
db.killOp(<opid>)
```

---

# 🌐 **14. Atlas Commands (CLI)**

```
atlas auth login
atlas clusters list
atlas clusters describe <name>
```

---
