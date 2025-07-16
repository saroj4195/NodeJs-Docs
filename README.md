hoisting 

const fs = require('fs');
fs.readFile('server.js', 'utf8', (err, data) => {
  if (err) throw err;
  console.log(data);
});


const path = require('path');
console.log(__dirname);                    // current folder
console.log(path.join(__dirname, 'test')); // /current/path/test


url - Parse URL

const url = require('url');
const myUrl = new URL('http://example.com:8000/path?name=John');
console.log(myUrl.hostname); // example.com
console.log(myUrl.pathname); // /path
console.log(myUrl.searchParams.get('name')); // John

 Quick interview notes

✅ Why Node is single-threaded yet handles many requests?
    Uses event loop + background workers (libuv) to do IO in parallel.

✅ How does require work?
    Loads module, caches it, returns module.exports.

✅ How to return JSON from Node HTTP server?
    Set header Content-Type: application/json and use JSON.stringify.

✅ What does __dirname give you?
    The absolute path to current directory.

