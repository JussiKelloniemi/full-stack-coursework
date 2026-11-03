# StudyBuddy

## Jussi Kelloniemi
<br>

Project is inside the Full-stack-project folder

## How to run
To run this project you need to install all the depenencies that are listed below in the dependencies section and setup the MongoDB database <br>
The front end can be built by using: 
```powershell 
npm run build
``` 
when in Full-stack-project/frontend directory. After that using:
```powershell
serve -s build
```
The front end is running in localhost 3000. <br>
The server must be running in the background which can be ran from the Full-stack-project using command:
```powershell
npm run server
```
After both of these are running the the user can access the page in http://localhost:3000.<br>
I did not use heroku to deploy the page because it required me to add credit card to use it.

# dependencies

## Backend

For backend has these dependencies:
- bcryptjs
- colors
- dotenv
- express
- express-async-handler
- jsonwebtoken
- mongoose

These need to be installed into the root folder by running this command:
```powershell
npm install bcrypt colors dotenv express express-async-handler jsonwebtoken mongoose
```

## Frontend
These dependencies need to be downloaded in the ./frontend directory:
- axios
- react
- react-dom
- react-icons
- react-rdux
- react-router-dom
- react-scripts
- react-tostify
- web-vitals
These can be installed by running this command:
```powershell
npm install axios react react-dom react-icons react-redux react-router-dom react-scripts react-toastify web-vitals
```
# .env configuration
This project needs to have .env file in the root folder. Values stored in that file are:
- NODE_ENV <br>
which is set to production
- PORT <br>
which sets the port where the backend is running and i have set it to 5000
- MONGO_URI <br>
Which is the connection string for the database for this project
-JWT_SECRET
Which is used to create token when registering and logging user. This can be set to any value but preferably to a long random one.

# MongoDB setup
MongoDB is used for this projects database. When running this project you need to create account for MongoDB Atlas and create new database. To connect it to the project you need to copy the connection string from the connection tab and add your password to <db_password> section of the string. This string needs to be then added to MONGO_URI in the .env file.