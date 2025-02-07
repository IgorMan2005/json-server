## JSON SERVER

1. npm i json-server

2. server.js

```
const jsonServer = require('json-server');
const server = jsonServer.create();
const router = jsonServer.router('db.json');
const middlewares = jsonServer.defaults();
const port = 8000;

server.use(middlewares);
server.use(router);

server.listen(port);
```

3. db.json

4. package.json

```
  "scripts": {
    "start": "node ./server.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
```

5. npm run start

6. GitHub репозиторий для json-server

<https://github.com/IgorMan2005/json-server>

git@github.com:IgorMan2005/json-server.git

```
echo "# json-server" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:IgorMan2005/json-server.git
git push -u origin main
```
