# ToxicBotList.js API Wrapper
![Hi](https://nodei.co/npm/tbl.js.png?downloads=true&stars=true)

A simple nodejs module helps you to get info/votes of bots from [Toxic Bot List](https://www.toxic-bot-list.ml)
# Setup
first, define module variable
```js
var tbl = require ('tbl.js');
```
Get info of bots by using getBot () function
```js
tbl.getBot ('BotID').then (async (BotInfo) => {
  console.log (BotInfo);
  // returns botInfo Object
});
```
Check if user has voted to the bot
```js
tbl.hasVoted ('BotID', 'UserID').then (async (BotInfo) => {
  console.log (BotInfo);
  // returns hasVoted boolean (true, false);
});
```
