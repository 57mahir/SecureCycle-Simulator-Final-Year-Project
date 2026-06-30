Requirements:
Node.js must be installed on your machine.

How to Run the Simulator: 
To run the application locally, you will need to start both the Backend server and the Frontend web interface. This requires opening two separate terminal windows.
Step 1: Start the Backend Server
Open a terminal and navigate to the backend folder:
cd backend
If the node_modules folder is missing, install the dependencies first:
npm install
Start the Express server:
node server.js
The backend API and game engine should now be running on http://localhost:3001.
Step 2: Start the Frontend Application
Open a second terminal window and navigate to the frontend folder:
cd frontend
If the node_modules folder is missing, install the dependencies first:
npm install
Start the Vite development server:
npm run dev
The web application will launch, typically accessible at http://localhost:5173 in your browser.

Accounts & Testing
Trainee Access:
You can create a standard trainee account directly through the Sign Up page on the main screen of the web application.
Administrator Access:
The application features a secure, role-based Admin Dashboard used for monitoring trainee metrics and inspecting raw database tables.
To create an admin account for testing purposes, navigate to the backend folder in your terminal and run:
node seedAdmin.js
You can then log in using:
Username: admin
Password: admin

Architecture & Data
Database: The application uses a local SQLite database (securecycle.sqlite). All interactions, event logs, and user data are stored here.
Live Traffic Engine: The simulation dashboard streams live dashboard traffic generated from the CMU datasets (final_http.csv and final_logon.csv) located in the backend folder.
