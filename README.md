# dockerBasicNode
Only creates a basic "Hello world app" with Node and Docker

## Local 
### 1. Crea un directorio local para nuestra App, con NPM generamos el archivo package.json e instalomos Express.

```
$ mkdir hello-world
$ cd hello-world
$ npm init
$ npm install —save express
```

### 2. Creamos un archivo index.js para nuestro codigo. 

`
$ touch index.js
`

### 3. Abrimos el archivo y creamos nuestra app web básica.

 ```javascript
var express = require('express')
var app = express()

app.get('/', function (req, res) {
  res.send('Hello World!')
})

app.listen(8081, function () {
  console.log('app listening on port 8081!')
})
 ```


