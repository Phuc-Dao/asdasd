# Developers Guild

Demo: <a href="https://stark-earth-96740.herokuapp.com/" target="_blank"> Click here</a>

A social media web app that allows developers to share their experiences and skills. This app features full user login and authentication and uses the github api to retrieve the top 5 projects from the developers repo. Below is a list of all the technologies used in this applications.

## Technologies Used

### Client Side

- **[React](https://github.com/facebook/react)**
- **[Redux](https://github.com/reactjs/redux)**
- **[Twitter Bootstap 4](https://github.com/twbs/bootstrap/tree/v4-dev)**
- **[React-Router-DOM](https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom)**

#### Libraries used in Client-side

-  **[axios](https://github.com/axios/axios)**
-  **[classnames](https://github.com/JedWatson/classnames)**
-  **[react-moment](https://github.com/headzoo/react-moment)**
-  **[react-redux](https://github.com/reduxjs/react-redux)**
-  **[redux-thunk](https://github.com/reduxjs/redux-thunk)**
-  **[validator](https://github.com/chriso/validator.js)**

### Server Side

-  **[Node.js / Express](https://github.com/expressjs/express)**
-  **[MongoDB](https://github.com/mongodb/mongo)**
-  **[JWT](https://github.com/auth0/node-jsonwebtoken)**
-  **[Passport](http://www.passportjs.org/)**
-  **[Passport-jwt](https://github.com/themikenicholson/passport-jwt)**

#### Libraries used in Server-side

-  **[bcryptjs](https://github.com/dcodeIO/bcrypt.js)**
-  **[bluebird](http://bluebirdjs.com/docs/getting-started.html)**
-  **[gravatar](https://github.com/emerleite/node-gravatar)**
-  **[mongoose](http://mongoosejs.com/)**
-  **[jwt-decode](https://github.com/auth0/jwt-decode)**
-  **[moment](https://momentjs.com/)**
-  **[validator](https://github.com/chriso/validator.js)**




<img src="screenshots/homepage.jpg">

---

## Quick Start

```bash
# clone repository
https://github.com/RoshanSureen/dev-connector.git

# Install dependencies
cd dev-connector && npm install

# create a .env file in root of your project
touch .env
```

In the .env file create the below 2 enviroment varieables. Make sure it is exactly as shown below. No special charecters or spaces must be there.

```
DB_URL=YOUR_OWN_MONGO_URI
TOKEN_SECRET=YOUR_OWN_SECRET
```

To run the development server:

```bash
# the development server runs on port 3000
npm run dev
```
To run production build:

```bash
# create code bundle
npm run build

# run production server
npm run prod
```

In the project a `Procfile` has also been provided. This file is used by Heroku.

### To deploy this project to heroku see steps below:

You will need to install the [heroku-cli](https://devcenter.heroku.com/articles/heroku-cli)

```bash
# Heroku-cli (paste link in browser)
https://devcenter.heroku.com/articles/heroku-cli
```

Afer installing heroku-cli run the following commands in terminal

```bash
# login locally
heroku login
```

You will be prompted to enter your email and password which is the same the email and password used when you sign up for Heroku

```bash
# create your app
heroku create

# set enviroment vareiables
heroku config:set DB_URL=YOUR_OWN_DB_URI
heroku config:set TOKEN_SECRET=YOUR_OWN_SECRET
```

Try to keep your production DB different from development DB

```bash
# bundle code for production
npm run build

# deploy code to heroku
git push heroku master:master
```

<img src="screenshots/signup.jpg">

---

<img src="screenshots/users.png">

---

<img src="screenshots/github.png">
