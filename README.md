<h1 align="center">Product Catalog System</h1>




-   ⚛️ Tech Stack: React.js, Node.js, Express.js, MongoDB, Chakra UI

### Setup .env file

```shell
MONGO_URI=your_mongo_uri
PORT=5000
```

### Run this app locally

```shell
npm run build
```

### Start the app

```shell
npm run start
```

### Guys in case u r getting the error: 

'NODE_ENV' is not recognized as an internal or external command,
operable program or batch file. 


1.npm install cross-env
2.Change the root package.json file  as: 
  "scripts": {
    "dev": "cross-env NODE_ENV=development nodemon backend/server.js",
    "build": "npm install && npm install --prefix frontend && npm run build --prefix frontend",
    "start": "cross-env NODE_ENV=production node backend/server.js"
  },
  
