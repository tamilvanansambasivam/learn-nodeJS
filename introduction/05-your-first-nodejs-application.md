### 05-your-first-nodejs-application.md

# Your First Node.js Application

Let’s create a simple "Hello, World!" application using Node.js.

## Code Example

### hello.js

```const http = require("http");

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader("Content-Type", "text/plain");
  res.end("Hello, World!\n");
});

const PORT = 3000;
server.listen(PORT, () => {
  console.log(`Server running at http://localhost:${PORT}/`);
});

```
