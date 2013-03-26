glove
=====

## For Node v0.10.x Users
Please recompile node modules and modify the package.json file

**Recompile node modules** remove /node_modules and reinstall [express](http://expressjs.com/), [socket.io](http://socket.io/) and [now](https://github.com/Flotype/now)

    rm -rf node_modules
    
    npm install express
    
    npm install socket.io
    
    npm install now
    

**Modify package.json**

Original: 

    {
      "name": "glove",
      "version": "0.0.1",
      "dependencies": {
          "now": "0.8.1",
          "socket.io": " 0.9.6"
      },
      "engines": {
        "node": "0.8.x",
        "npm": "1.1.x"
      }
    } 
    
Modified:

    {
      "name": "glove",
      "version": "0.0.1",
      "dependencies": {
          "now": "0.8.1",
          "socket.io": " 0.9.x"
      },
      "engines": {
        "node": "0.10.x",
        "npm": "1.2.x"
      }
    }

