writeCode

Run these shell commands in mongo shell:

- db.version()
- db.stats()
- db.help()

Write code to

- create a database of your country name.
```
 db.createCollection("India", {size: 29, capped: true});
```
- check list of databases to see newly created database.
```
    db.getCollectionNames();
```
- check which database you are currently connected to ?

