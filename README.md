# Online-Outpass-Management-System
This Outpass Management System is designed for educational institutions to manage student departures from campus. It ensures timely communication with wardens and authorities. The system supports multiple users simultaneously, offers high-level security to prevent unauthorized access, and is network-based for real-time updates.
Leave Management System
A web-based Leave Management System designed for students, wardens, and HODs to manage leave requests in a seamless and structured way.

Features
User Authentication: Supports role-based login for students, wardens, and HODs using Passport.js.
Leave Requests:
Students can apply for leave.
Wardens and HODs can view, approve, or reject leave requests.
Role-Specific Dashboards:
Students can view their profile, leave status, and apply for leave.
Wardens and HODs can view pending leave requests for their department or hostel.
Validation: Ensures all form inputs are properly validated using express-validator.
Date Management: Handles and displays dates elegantly using the Moment.js library.
Dynamic Views: Powered by EJS for responsive, dynamic templates.
Technologies Used
Node.js: Backend runtime.
Express.js: Web framework.
MongoDB: Database for storing users, leave requests, and other data.
Mongoose: ORM for MongoDB.
Passport.js: Authentication middleware.
Moment.js: Date and time management.
EJS: Template engine for rendering views.
Installation and Setup
Prerequisites
Ensure you have the following installed on your system:

Node.js (v14 or above)
MongoDB (local or cloud-based like MongoDB Atlas)
Steps to Run the Project
Clone the Repository:

bash
Copy code
git clone https://github.com/yourusername/LeaveApp.git
cd LeaveApp
Install Dependencies:

bash
Copy code
npm install
Configure Environment Variables:

Create a .env file in the root directory.
Add the following variables:
makefile
Copy code
DATABASE_URL=mongodb://localhost:27017/LeaveApp
SESSION_SECRET=your_secret_key
Start the Server:

bash
Copy code
node app.js
The server will start on http://localhost:3005.

Access the Application: Open your browser and go to http://localhost:3005.

Project Structure
bash
Copy code
LeaveApp/
├── models/          # Mongoose schemas for database collections
│   ├── student.js
│   ├── warden.js
│   ├── hod.js
│   ├── leave.js
├── public/          # Static files (CSS, images, JS)
│   └── css/
│       └── styles.css
├── routes/          # Route handlers for different roles
│   ├── index.js
│   ├── students.js
│   ├── hods.js
│   ├── wardens.js
├── views/           # EJS templates for rendering pages
│   ├── register.ejs
│   ├── profilestud.ejs
│   ├── homestud.ejs
├── .env             # Environment variables (excluded in .gitignore)
├── .gitignore       # Files to ignore in version control
├── README.md        # Project documentation
├── app.js           # Main entry point of the application
├── package.json     # Project metadata and dependencies
└── package-lock.json
Usage
Students:
Register and log in.
Apply for leave, view leave history, and profile.
Wardens:
View pending leave requests from students in their hostel.
Approve or reject leave applications.
HODs:
View department-wise leave requests.
Approve or reject leave applications.
Contributing
Contributions are welcome! Please follow these steps:



