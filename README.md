Automobile Inventory System
This is a web-based Automobile Inventory System designed for seamless management of automobile data. It includes user authentication, a dashboard, profile management, and the ability to add, view, and manage automobiles.

Features
User Authentication: Signup and login functionalities.
User Dashboard: View and manage automobile inventory.
Add New Automobiles: Input automobile data into the inventory.
Responsive Design: Optimized for various screen sizes.

Technologies Used
Backend:
Node.js: JavaScript runtime for server-side development.
Express.js: Web framework for building the API.
PostgreSQL: Relational database for storing user and automobile data.
bcrypt.js: Password hashing for secure user authentication.
jsonwebtoken: For generating and verifying user tokens.
Frontend:
HTML5, CSS3: For building the user interface.
Vanilla JavaScript: Client-side scripting for interactivity.
Responsive Design: Ensures compatibility across devices.

File Structure

project/
├── backend/               
│   └── db.js
│   ├── routes/                
│   │   ├── auth.js           
│   │   ├── inventory.js      
│   │   ├── admin.js
│   ├── server.js              
│   └── package.json           
├── frontend/
│   │   │   └── style.css      
│   │       └── main.js        
│   │   ├── index.html         
│   │   ├── signup.html        
│   │   ├── home.html
│   │   ├── dashboard.html    
│   │   ├── admin-dashboard.html 
│   │   ├── add-car.html     
└── README.md      

Installation and Setup

Prerequisites:
Node.js installed on your computer.
PostgreSQL database setup.
A code editor (e.g., VSCode).
Steps:
Clone the repository:

git clone https://github.com/your-username/automobile-inventory-system.git
cd automobile-inventory-system
Navigate to the backend directory:

cd backend
Install backend dependencies:

npm install
Configure the database:

Open backend/config/db.js and update the database credentials.
Run database migrations (if any):

psql -U your_user -d automobile_inventory -f migrations.sql
Start the backend server:

npm start
Open a new terminal and navigate to the frontend directory:

cd frontend
Open index.html in your browser to view the application.

API Endpoints
Authentication:
POST /auth/signup: Register a new user.
POST /auth/login: Authenticate an existing user.
Dashboard:
GET /dashboard: Retrieve user dashboard data.
Automobiles:
POST /automobiles/add: Add a new automobile to the inventory.
GET /automobiles: Retrieve all automobiles.
