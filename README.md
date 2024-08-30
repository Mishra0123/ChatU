# ChatU

# Introduction

This repository consists of a Chat Application built with the MERN stack
(MongoDB, Express.js, Node.js, and React.js).

This is a full-stack chat application that can be up and running with just a few steps. Its frontend is built with [Material UI](https://mui.com/material-ui/) running on top of [React](https://react.dev/). The backend is built with [Express.js](https://expressjs.com/) and [Node.js](https://nodejs.org/en). Real-time message broadcasting is developed using [Socket.IO](https://socket.io/).

# Features

This application provides users with the following features:

- **Authentication** using [JWT Tokens](https://jwt.io/).
- A **Global Chat** which can be used by anyone using the application to broadcast
  messages to everyone else.
- A **Private Chat** functionality where users can chat with other users privately.
- **Real-time updates** to the user list, conversation list, and conversation
  messages.

## Screenshots

### Register
![Screenshot 2023-09-28 120018](https://github.com/AaryaaRam/ChatU/assets/95530767/0d8b9c7c-3573-468e-9143-0c6d26f5eb13)

### Login
![Screenshot 2023-09-28 115959](https://github.com/AaryaaRam/ChatU/assets/95530767/aa509e39-4291-43ad-926b-48d4c24a25b0)

### Private Chat
![Screenshot 2023-09-28 120459](https://github.com/AaryaaRam/ChatU/assets/95530767/b6fc601b-42c9-4184-8bc1-e8cce58df956)

![Screenshot 2023-09-28 120536](https://github.com/AaryaaRam/ChatU/assets/95530767/c06b1f5f-fbeb-4ce0-9ce2-a07b53ee5ba6)

### Global Chat
![Screenshot 2023-09-28 120441](https://github.com/AaryaaRam/ChatU/assets/95530767/c129cfb5-6924-40ec-a085-456b333f1bcc)

# How to use

You can have this application up and running with just a few steps because it has both the frontend and the backend in a single repository. Follow the steps below to do so:

1. Clone this repo  
   ```git clone https://github.com/AaryaaRam/ChatU.git```
2. Once you have the repo, you need to install its dependencies. So using a
   terminal, move into the root directory of the project (```cd ChatU```) and execute ```npm install``` to install the dependencies of the Node.js server and then run 
   ```npm run client-install``` to install the dependencies of the frontend or client. The second command is a custom command that I wrote to simplify the installation process.
3. This application uses MongoDB as its Database. So make sure you have it installed. You can find detailed guide on how to do so [here](https://www.mongodb.com/docs/manual/administration/install-community/). Once installed, make sure that your local MongoDB server is not protected by any kind of authentication. If there is authentication involved, make sure you edit ```mongoURI``` in the ```config/keys.js``` file.  
**NOTE:** Use the ```npm audit fix --force``` command to address any errors or vulnerabilities that may have occurred during the installation of the dependencies.
4. Finally, all you have to do is simply run ```npm run dev```. If this command
   fails, try installing the package [concurrently](https://www.npmjs.com/package/concurrently) globally by running ```npm install -g concurrently``` and then running the ```dev``` command.
5. The frontend of the application will automatically open in your web browser, and you can test it right away.

# Things to note

* The frontend is built using [create-react-app](https://create-react-app.dev/).
* Backend database connections are managed through [Mongoose ORM](https://mongoosejs.com/).
* Code quality is ensured using [ESlint](https://eslint.org/).
* Passwords are securely hashed using the [bcrypt.js](https://www.npmjs.com/package/bcrypt) library before being stored in the database.
* String inputs are validated and sanitized with the help of [validator.js](https://www.npmjs.com/package/validator) library to ensure maximum security.
* User authentication is handled through the [passport](https://www.npmjs.com/package/passport) middleware along with [JWT tokens](https://jwt.io/).


