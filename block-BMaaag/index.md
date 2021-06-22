writeCode

Write code to:-

- create a database named `mountains`
```js
    use mountains
```

- a collection inside that database named `himalayas`
```js
    db.createCollection("himalayas");
```

- insert 1 document into that collection `{name: 'Dhauldhar range', height: '4000 mtrs'}`
```js
    db.himalayas.insert(
            {
                name: 'Dhauldhar range', 
                height: '4000 mtrs'
            }
        );
```

- insert multiple document using insertMany command
```js
        db.himalayas.insertMany( [
            {
                name: 'Dhauldhar range', 
                height: '4000 mtrs'
            },
            {
                name: 'Karakoram range', 
                height: '8000 mtrs'
            },
            {
                name: 'Jansker range', 
                height: '6000 mtrs'
            },
        ]);
```

- find all documents from mountains
```js
    db.himalayas.find().pretty();
```

- find a single document using name
```js
   db.himalayas.find({name: "Jansker range"}).pretty(); 
```