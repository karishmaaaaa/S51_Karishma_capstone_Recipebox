🍽️ Recipe Box

A full-stack MERN application where users can browse, create, and manage food recipes.
Built with MongoDB, Express.js, React, and Node.js, it includes user authentication, recipe CRUD operations, and a modern, responsive UI.

🚀 Features

🔐 User Authentication – Secure signup and login using JWT.

🍳 Recipe Management – Create, edit, delete, and view recipes.

🖼️ Image Uploads – Add photos to your recipes.

🔍 Search & Filter – Find recipes by name, category, or ingredients.

💾 User Dashboard – Manage your personal recipes.

📱 Responsive UI – Works beautifully on desktop and mobile.

🛠️ Tech Stack
Layer	Technologies
Frontend	React, React Router, Axios, Tailwind CSS / CSS Modules
Backend	Node.js, Express.js
Database	MongoDB (Mongoose)
Authentication	JSON Web Tokens (JWT), bcrypt
Image Upload (optional)	Cloudinary / Multer
⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/yourusername/recipe-box.git
cd recipe-box

2️⃣ Install dependencies
# Install server dependencies
cd server
npm install

# Install client dependencies
cd ../client
npm install

3️⃣ Add environment variables

Create a .env file inside the server directory with the following:

MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
CLOUD_CLOUD_NAME=your_cloud_name (optional)
CLOUD_API_KEY=your_api_key (optional)
CLOUD_API_SECRET=your_api_secret (optional)

4️⃣ Run the app
# Run backend (in server/)
npm run dev

# Run frontend (in client/)
npm start

📁 Folder Structure
recipe-box/
│
├── client/                # React frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
│
├── server/                # Express backend
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   └── package.json
│
└── README.md

🧑‍🍳 Usage

Sign up or log in to your account.

Create new recipes with a title, description, ingredients, and an image.

Browse and search recipes by name, category, or ingredient.

Edit or delete your recipes anytime from your dashboard.

🔒 Authentication Flow

User signs up or logs in via the React frontend.

Credentials are validated on the Express backend.

A JWT token is generated and stored securely (HTTP-only cookie or local storage).

Protected routes verify the token via authentication middleware.

🌩️ Image Upload Options
Using Cloudinary

Add your Cloudinary credentials in .env.

Images will be uploaded and hosted on Cloudinary.

Using Multer

Images will be saved locally in /uploads inside the backend folder.

📡 API Routes


🔐 Auth Routes
Method	Endpoint	Description
POST	/api/auth/register	Register a new user
POST	/api/auth/login	Log in and get a JWT token


🍳 Recipe Routes

GET	/api/recipes	Get all recipes
GET	/api/recipes/:id	Get a single recipe by ID
POST	/api/recipes	Create a new recipe
PUT	/api/recipes/:id	Update an existing recipe
DELETE	/api/recipes/:id	Delete a recipe

🧰 Available Scripts

In the client/ directory
Command	Description
npm start	Runs the frontend in development mode
npm run build	Builds the frontend for production
npm test	Runs tests

In the server/ directory
Command	Description
npm run dev	Starts the backend with Nodemon
npm start	Starts the backend normally
📸 Screenshots (Optional)

Add screenshots or GIFs of your app here to showcase its UI.

💡 Future Improvements

🌐 Social login (Google / GitHub)

⭐ Recipe rating and comments

❤️ Favorite and share recipes

🌓 Dark mode support

🏗️ Contributing
