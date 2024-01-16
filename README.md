# Pizza Time
## Getting Started with Create React App <a id="gettingStarted"></a>

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

To get started you need to:

1. Clone the project
2. npm install
3. Install listed dependencies
4. Use available scripts, like npm start

## Instructions <a id="instructions"></a>

- When you fork or download the project install node modules using npm install and then any additonal dependencies you don't have from <a id="dependencies">Dependencies</a> list

- Next, you need to create the file name .env located outside src file

- In the .env file I am using several variables:
1. REACT_APP_DATABASE_URL & MYSQL_ATTR_SSL_CA - these variables contain information that will connect you to the PlanetScale database. You can use the following documentation https://planetscale.com/docs/tutorials/connect-nodejs-app. If you use any other database you need to use the accoridng information to connect to that database. 
Note that the table for users in my case is named "users" and contains columns with the following data: id | email | password | fullname | address | number.
2. REACT_APP_USERS_URL - these is a url for Node.js server. First, it's better to run it locally and only then switch to whatever you want. If you want to run the server locally the value of this variable should be http://localhost:3000/users. In this project I set up backend using Vercel. You can google "How to Deploy Your Node.js Backend Project to Vercel" and set up your own backend.
3. REACT_APP_CAPTCHA_URL - the same logic works for this backedn url which this time is used for captcha verification. Locally, the url value should be http://localhost:3000/verify-recaptcha.
4. REACT_APP_CAPTCHA_KEY & REACT_APP_CAPTCHA_SECRET - both values can be found once you create an account for reCaptcha at https://www.google.com/recaptcha/about/. Please use their documentation for better understanding.

- Once you set up the variables, you can run the server on one port, if you use local server and the website on another port. 

## Available Scripts <a id="scripts"></a>

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.
