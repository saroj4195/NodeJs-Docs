hoisting 

const fs = require('fs');
fs.readFile('server.js', 'utf8', (err, data) => {
  if (err) throw err;
  console.log(data);
});

