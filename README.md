hoisting 

const fs = require('fs');
fs.readFile('server.js', 'utf8', (err, data) => {
  if (err) throw err;
  console.log(data);
});

const path = require('path');

console.log(__dirname);                    // current folder
console.log(path.join(__dirname, 'test')); // /current/path/test

