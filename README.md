提供一套更適合懶人的 Behance API 介面懶人包。

## Usage
#### Initialize
First install from NPM.
```sh
$ npm install be-simple --save
```
Register your application at [Behance Dev](https://www.behance.net/dev/register)
```js
var Be = require('be-simple');
var be = new Be(YOUR_CLIENT_ID);
```
### User

##### Get a user's basic info
```js
be.user(USER_ID, function(data) {
	console.log(data);
})
```

##### Get a user's projects
```js
be.userProjects(USER_ID, function(data) {
	console.log(data);
})
```

##### Get all followers of a user
Please be careful when calling this method.
```js
be.userAllFollowers(USER_ID, function(followers) {
	console.log(followers);
})
```

##### Get all followings of a user
Please be careful when calling this method.
```js
be.userAllFollowings(USER_ID, function(followings) {
	console.log(followers);
})
```

##### Get a user's statics
```js
be.userStats(USER_ID, function(data) {
	console.log(data);
})
```