 ## OShop
### Install Dependencies
```sh
$ npm install 
```
### Create a new firebase project
Login into your google account and create a new firebase project [here](https://console.firebase.google.com/u/0/)

Create a `.env.prod` file for production and `.env.dev`for development in the root of your project folder
and add the following configuration details. It can be found on your firebase project.

```
FIREBASE_API_KEY=
FIREBASE_AUTH_DOMAIN=
FIREBASE_DB_URL=
FIREBASE_PROJECT_ID=
FIREBASE_STORAGE_BUCKET=
FIREBASE_MSG_SENDER_ID=
FIREBASE_APP_ID=

```

### Run development server
```sh 
$ npm run dev-server
```

### Build the project
```sh
$ npm run build
```

### How to perform CRUD operations for Admin
1. Inside `src/routers/AppRouter.js` uncomment all code related to admin.
2. Inside `src/reducers/authReducer.js`, change the initState type value from 'client' to 'admin'. Delete `initState` variable if you want to authenticate client.
3. Delete persisting auth state in localStorage if one exists.
 

### Features

* Admin CRUD operations
* Firebase authentication
* Firebase auth provider authentication
* Account creation and edit

