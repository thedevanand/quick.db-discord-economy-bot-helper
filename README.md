<h1>QUICK.DB DISCORD BOT HELPER</h1>
<h5>This repository is made for people who are beginner to discord bots wanting to make discord economy bots.</h5>

You'll need a package named [**Quick.db**](https://www.npmjs.com/package/quick.db).

```js
// to install the package
npm install quick.db
or
npm i quick.db
```

---
Require the package where ever you want to use the database. 

```js
const db = require('quick.db');
```


---
To set a value use - 

```js
db.set('key', value);

// example
user = ClientUser; // should be an user object

db.set(`balance_${user.id}`, 2000); // its economy so you will use an integer as value
```


---
To get a value use - 

```js
db.get('key');

// example
user = ClientUser; // should be an user object

db.get(`balance_${user.id}`); // 2000

// or

db.fetch(`balance_${user.id}`); // 2000

```


---
To make addition in a value use - 

```js
db.add('key', value);

// example
user = ClientUser; // should be an user object

db.add(`balance_${user.id}`, 2000);
```


---
To make subtraction in a value use - 

```js
db.subtract('key', value);

// example
user = ClientUser; // should be an user object

db.subtract(`balance_${user.id}`, 2000);
```


---
To remove a key use - 

```js
db.remove('key');

// example
user = ClientUser; // should be an user object

db.remove(`balance_${user.id}`);
```

**NOTE** : That subtract and remove can confuse you, so double check your code every time you are subtracting.


**THIS DOCUMENT IS STILL NOT COMPLETED YET, WE MAY COMMIT CHANGES IN FUTURE**

`Version : 1.0.0`

```
THANKS FOR READING THIS DOCUMENT - DEV ANAND
```
