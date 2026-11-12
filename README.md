# StudyBuddy

## Jussi Kelloniemi
<br>

Project is inside the Full-stack-project folder

## How to run step by step
1. Clone repository
   Run this command in your terminal to clone this repository and go to correct directory:
   ```powershell
   git clone https://github.com/JussiKelloniemi/full-stack-coursework.git
   ```
   ```powershell
   cd full-stack-coursework
   ```
   ```powershell
   cd Full-stack-project
   ```
2. Install backend and frontend dependencies
   When inside the root folder of the project "Full-stack-project" run this to install backend dependencies
   ```powershell
   npm install bcryptjs colors dotenv express express-async-handler jsonwebtoken mongoose
   ```
   Then change to frontend directory:
   ```powershell
   cd frontend
   ```
   And run this:
   ```powershell
   npm install axios react react-dom react-icons react-redux react-router-dom react-scripts react-toastify web-vitals
   ```
3. Setup MongoDB
   MongoDB is used for this projects database. When running this project you need to create account for MongoDB Atlas and create new database. To connect it to the project you need to copy the connection string from the connection tab and add your password to <db_password> section of the string. This string needs to be then added to MONGO_URI in the .env file.
4. Configure .env file
  This project needs to have .env file in the root folder. Values stored in that file are:
  - NODE_ENV <br>
  which is set to production
  - PORT <br>
  which sets the port where the backend is running and i have set it to 5000
  - MONGO_URI <br>
  Which is the connection string for the database for this project
  - JWT_SECRET <br>
  Which is used to create token when registering and logging user. This can be set to any value but preferably to a long random one.
5. Run backend & frontend<br>
  In the root folder run these commands:
  First:
  ```powershell
  npm run build --prefix frontend
  ```
  Second:
  ```powershell
  npm run server
  ```
Page is now should now be available at http://localhost:5000 ready to be used

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
npm install bcryptjs colors dotenv express express-async-handler jsonwebtoken mongoose
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

