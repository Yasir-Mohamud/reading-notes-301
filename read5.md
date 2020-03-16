# Heroku Deployment
- Node.js  is an open source where we can create networking apps and servers.
- To make a server you need to use this javascript code :

``` js
var http = require("http");

http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("It's alive!");
  response.end();
}).listen(3000);
```

this makes a server and to make live you go to your terminal and type 

```
node <name of js file> .js
```

Heroku is a cloud application that deploys your web server and turns it from a local server to a world wide srever.

