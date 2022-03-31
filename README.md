
local
#  ng serve

github--heroku
-- https://github.com/andreasrothbern/6trlfn--run
-- https://dashboard.heroku.com/apps/angular-6trlfn-run

1. install express
# npm i express --save
3. server.js
--
const express = require('express');
const path = require('path');
const app = express();
app.use(express.static(__dirname + '/dist/<app-name>'));
app.get('/*', function(req,res) {
res.sendFile(path.join(__dirname+
'/dist/<app-name>/index.html'));});
app.listen(process.env.PORT || 8080)
--
4. Test 
# node server.js

