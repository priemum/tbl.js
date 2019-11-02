# ToxicBotList.js API Wrapper
![Hi](https://nodei.co/npm/tbl.js.png?downloads=true&stars=true)

A simple nodejs module helps you to get info/votes of bots from [Toxic Bot List](https://www.toxic-bot-list.ml)
# Setup and Examples
first, define module variable
```js
var tbl = require ('tbl.js');
```
Get info of bots
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
# botInfo Object
returns Object contains: 
```js
id: String // Bot userid
username: String // Bot username
avatar: String // Bot avatarUrl
lib: String // Library of bot
prefix: String // Prefix of bot
shortdesc: String // Short description of bot in TBL site
longdesc: String // Long description of bot in TBL site (contains markdown & html)
support: String or Boolean // Support invite url , if doesn't returns false
owner: Object // Owner object contains (id, name)
invite: String // Invite link of the bot (perms 8)
verified: Boolean // returns true if bot is verified and false if not
widget: String // widget api image url of bot in TBL
votesCount: Number // returns the size of votes
hasVoted: Object // Object of all votes in lifetime with timestamp of it
```
