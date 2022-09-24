# To run application locally use concurrenlty command in scripts -> package.json

    "server": "nodemon server.js",
     "client": "cd client && npm start",
    "start": "concurrently \"npm run server\" \"npm run client\""


# While uploading production build to server use the below command in scripts -> package.json

 "start": "node server.js",
 "heroku-postbuild": "cd client && npm install && npm run build"