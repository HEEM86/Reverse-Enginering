# Reverse-Enginering

<a href="https://ibb.co/cvyF1zF"><img src="https://i.ibb.co/dcf2rn2/passport.png" alt="passport" border="0"></a>


# Description

This assignment provides code for an opt-in sign-up / login application. In this README will do some reverse-engineering which consists of reviewing and providing a summary of how the application works. 

The application is using bcrypt to create a secured environment, for the user to enter the information and PassPort and Sequelize is handling the authentication. 

 # Walk Through

 **Server.js**

 server.js requires packages (dependencies) to execute, for this case this application needs express, express-session and passport. In addition it creates the routes and establishes the database along with the PORTs connnect and communicate with the server.


**isAuthenticated.js** 

Is middleware framework that verifies registered users.

**Config.json**

A authentication database that stores members login access for verification when they login

**Passport.js**

Is a gate keeper that checks the user login values and local strategy verifies and prompted to either the members page if successful or an alert that the values enter are incorrect

**login.html**

Displays an opt-in with login values and buttons that execute to the desired route

**members.html**

This is the members only layout, where memebers have access to exculsive information. There's also buttons to allow the user to sign-out 

**signup.html**

Contains the form that allows users to enter their login values.

**login.js**

Captures the users login values and directs them to members.html if their password passed the verification.

**members.js**

Updates the member with their name and email after they've logged in.

**signup.js**

Captures and stores user login credentials and directs the user to members.html

**html-routes.js**

Checks the user accordingly, by directing registered users to the members page or redirects new users to the sign-up page

**api-routes.js**

Has the active user's information which is displayed when signing in or out.

**index.js**

Establishes communication with the data base and imports user log information.

**users.js**

Creates the bcrypt secure environment


## Author :pen:

Ernest Wesson :zap:

LinkedIN: https://www.linkedin.com/in/ernest-wesson-b4183b5a/



## License :clipboard:


MIT License

Copyright (c) [2020] [Ernest]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.









