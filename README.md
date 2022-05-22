Codigo en JavaScript para desplegr un servidor que escucha en el puerto 8080

1. Debe copiar el siguiente código en un archivo llamado server.js

/*-----------------------------------------------------*/
'use strict';

const express = require('express');

const PORT = 8080;
const HOST = '0.0.0.0';

const app = express();
app.get('/', (req, res) => {
  res.send('Hello World Node JS Server ');
});

app.listen(PORT, HOST);
console.log(`Running on http://${HOST}:${PORT}`);
/*-----------------------------------------------------*/

