# ToxicBotList.js API Wrapper
![Hi](https://nodei.co/npm/tbl.js.png?downloads=true&stars=true)

A simple nodejs module helps you to get info/votes of bots from [Toxic Bot List](https://www.toxic-bot-list.ml)
# Examples:
```js
var tbl = require ('tbl.js');

tbl.getBot ('BotID').then (async (BotInfo) => {
  console.log (BotInfo);
  // returns botInfo Object
});


tbl.hasVoted ('BotID', 'UserID').then (async (BotInfo) => {
  console.log (BotInfo);
  // returns hasVoted boolean (true, false);
});
```
