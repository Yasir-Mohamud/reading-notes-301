# NODE 

- Is a  asynchronous event-driven JavaScript runtime.
- You can run js code in the terminal by writing as  ``` node <thefile.js> ```.
- You can create a package.json by running ``` npm init -y ``` in the terminal.
- Node.js lets us run js in the server.
- This an example of how to create a server 
``` js
const http = require('http');

http.createServer((request, response) => {
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);

console.log('Server running on http://localhost:3000');
```

- How Node.js works is the Node apps pass an event with a callback function. 
- Then the event loop creates threads and manages them and executes the task that was given .
