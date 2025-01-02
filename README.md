# Login and Registration Form

## Project Description
This project is a web-based application that provides a simple login and registration form. Users can register with their details and log in to access the application. The project is built using React for the frontend, Node.js for the backend, and MySQL as the database.

## Installation Guide

### Prerequisites
- Ensure you have [Node.js](https://nodejs.org/) installed on your system.
- Install [MySQL](https://www.mysql.com/) and set up a database.
- Install a code editor like [Visual Studio Code](https://code.visualstudio.com/).

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd gkb_anu
   ```

2. Install dependencies for the frontend:
   ```bash
   cd frontend
   npm install
   ```

3. Set up the backend (instructions not provided in this README; ensure you have a backend folder with Node.js and MySQL configurations).

4. Start the development server:
   ```bash
   npm start
   ```

5. To compile code is  : ``` npm run dev ```

8.   Open the application in your browser at  http://localhost:5173/.
```

### NOTE :
 ```
 please extract frontend and server folder and open it in vscode.
 open a New terminal > select the option command  prompt under the dropdown of powershell
                     > cd frontend
                     > npm run dev
you will be getting the url in order to view the register Form.                     
```

### Frontend page design
```
Below link is the link please copy and paste in the chrome so that the register page will be displayed.
link - https://github.com/user-attachments/assets/85d595b9-4890-413e-ae7d-0cc6dbaf4b05
```
### Used Frameworks

- **Frontend:** React, TailwindCSS
- **Backend:** Node.js, Express.js
- **Database:** MySQL
```
### Responsive Design:
```
The frontend is designed to work seamlessly on different screen sizes Built With
Frontend:
  React.js : Tailwind CSS (for styling)
  Backend: Node.js & Express.js
  
Database:
 MySQL
 Authentication:
 bcrypt (password hashing)
 JSON Web Tokens (JWT)
 ```

## Project Structure
```
gkb_anu/
  ├── frontend/                          # React frontend folder
  │   ├── node_modules/                  # Contains installed dependencies for frontend
  │   ├── src/                            # Source code for the React app
  │   │   ├── assets/                     # Static files like images
  │   │   │   └── react.svg               # Example image asset
  │   │   ├── pages/                      # React pages
  │   │   │   ├── Home.jsx                # Home page component
  │   │   │   ├── Login.jsx               # Login page component
  │   │   │   └── Register.jsx            # Register page component
  │   │   ├── App.jsx                     # Main app component
  │   │   ├── index.css                   # Global CSS
  │   │   ├── main.jsx                    # Entry point for React app
  │   │   └── vite.config.js              # Vite configuration file for frontend
  │   ├── .gitignore                      # Git ignore file to exclude node_modules, build files, etc.
  │   ├── eslint.config.js                # ESLint configuration file
  │   ├── index.html                      # Basic HTML template for the app
  │   ├── package-lock.json               # Lock file for npm packages
  │   ├── package.json                    # Defines project dependencies and scripts for frontend
  │   ├── postcss.config.js               # PostCSS configuration with TailwindCSS and Autoprefixer
  │   ├── vite.config.js                  # Vite configuration file
  │   └── tailwind.config.js              # TailwindCSS configuration file
  └── server/                             # Backend server folder
      ├── node_modules/                   # Contains installed dependencies for the backend (express, etc.)
      ├── index.js                        # Express server setup
      ├── package-lock.json               # Lock file for backend npm packages
      └── package.json                    # Defines backend dependencies and scripts
```
Here’s a concise description of each file in the folder structure :
### **Frontend Folder (`frontend/`)**
```
```
1. Node_modules
Contains installed dependencies (managed by npm) for the frontend application, such as React, Vite, TailwindCSS, etc.
```
```
2. src  
   The source code for the React app, where all React components, pages, and assets are stored.

   - assets  
     Contains static files like images, e.g., `react.svg`.

   - pages  
     Holds React page components:
     - Home.jsx : A component for the home page.
     - Login.jsx : A component for the login page.
     - Register.jsx : A component for the register page.

   - App.jsx
     The main React component that serves as the root of the application.

   - index.css  
     Contains global styles for the React application, including any necessary CSS for TailwindCSS.

   - main.jsx 
     The entry point of the React application that renders the `App.jsx` component.

3. .gitignore
   Specifies files and directories to be ignored by Git (e.g., `node_modules/`, build files, etc.).

4. eslint.config.js 
   Configures ESLint to enforce coding standards and rules for JavaScript and React code. It includes rules for React, hooks, and JSX runtime.

5. index.html
   The basic HTML template that Vite uses to serve the React app. It includes references to the root `div` and the `main.jsx` entry script.

6. package-lock.json
   Automatically generated when running `npm install`, it locks down the exact versions of dependencies installed, ensuring consistency across 
   environments.

7. package.json 
   Contains metadata about the project (name, version, description) and lists frontend dependencies (like React, Vite, TailwindCSS), scripts, 
   and other configurations.

8. postcss.config.js 
   Configures PostCSS with TailwindCSS and Autoprefixer for processing CSS files.

9. vite.config.js
   Configures Vite as the build tool for the React app. It includes plugins such as `@vitejs/plugin-react` to support React features.

10. tailwind.config.js
    Configures TailwindCSS, specifying which files Tailwind should scan for class names (e.g., `index.html` and `src/`).

11. README.md
    A basic template for project documentation, providing instructions on how to set up, install dependencies, and run the project.

---

### Server Folder (`server/`)

1. Node_modules 
   Contains installed dependencies for the backend (e.g., `express`), managed by npm.

2. index.js 
   The entry point for the Express server. It sets up the server, defines basic routes, and starts listening on port 3000.

3. package-lock.json 
   Automatically generated when running `npm install`, it locks the versions of backend dependencies to ensure consistency.

4. package.json
   Defines metadata about the backend server (name, version, etc.) and lists the server dependencies (e.g., `express`). It also includes 
   scripts, like `"start": "node index.js"`, to run the backend server.

```
## FRONTEND FOLDER CONTAINS :-
```
### react.svg  
```
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
```
```
### Home.jsx
```
```javascript
import React from 'react';

const Home = () => {
    return (
        <div className='text-3xl text-blue-500'> Home </div>
    );
};

export default Home;
```

### Login.jsx
```javascript
import React from 'react';

const Login = () => {
    return (
        <div>Login</div>
    );
};

export default Login;
```

### Register.jsx
```javascript
import React from 'react';
import { Link } from 'react-router-dom';
import axios from 'axios';

const Register = () => {
    return (
        <div className='flex justify-center items-center h-screen'>
            <div className='shadow-lg px-8 py-5 border w-96'>
                <h2 className='text-lg font-bold mb-4'>Register</h2>
                <form>
                    <div className="mb-4">
                        <label htmlFor="username" className='block text-gray-700'> Username </label>
                        <input type="text" placeholder='Enter Username' className='w-full px-3 py-2 border' name="username" />
                    </div>
                    <div className="mb-4">
                        <label htmlFor="email" className='block text-gray-700'> Email </label>
                        <input type="email" placeholder='Enter Email' className='w-full px-3 py-2 border' name="email" />
                    </div>
                    <div className="mb-4">
                        <label htmlFor="password" className='block text-gray-700'> Password </label>
                        <input type="password" placeholder='Enter Password' className='w-full px-3 py-2 border' name="password" />
                    </div>
                    <button className="w-full bg-green-600 text-white py-2"> Submit </button>
                </form>
                <div className="text-center">
                    <span>Already have account?</span>
                    <Link to='/login' className='text-blue-500'>Login</Link>
                </div>
            </div>
        </div>
    );
};

export default Register;
```

### App.jsx
```javascript
import { BrowserRouter, Routes, Route } from 'react-router-dom';
import Home from './pages/Home';
import Register from './pages/Register';
import Login from './pages/Login';

function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path='/' element={<Home />}></Route>
        <Route path='/register' element={<Register />}></Route>
        <Route path='/login' element={<Login />}></Route>
      </Routes>
    </BrowserRouter>
  );
}

export default App;
```

### index.css
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### main.jsx
```javascript
import { StrictMode } from 'react';
import { createRoot } from 'react-dom/client';
import './index.css';
import App from './App.jsx';

createRoot(document.getElementById('root')).render(
  <StrictMode>
    <App />
  </StrictMode>,
);

### .gitignore
```
node_modules/
dist/
.vite/
.env
```

### eslint.config.js
js
```
import js from '@eslint/js'
import globals from 'globals'
import react from 'eslint-plugin-react'
import reactHooks from 'eslint-plugin-react-hooks'
import reactRefresh from 'eslint-plugin-react-refresh'

export default [
  { ignores: ['dist'] },
  {
    files: ['**/*.{js,jsx}'],
    languageOptions: {
      ecmaVersion: 2020,
      globals: globals.browser,
      parserOptions: {
        ecmaVersion: 'latest',
        ecmaFeatures: { jsx: true },
        sourceType: 'module',
      },
    },
    settings: { react: { version: '18.3' } },
    plugins: {
      react,
      'react-hooks': reactHooks,
      'react-refresh': reactRefresh,
    },
    rules: {
      ...js.configs.recommended.rules,
      ...react.configs.recommended.rules,
      ...react.configs['jsx-runtime'].rules,
      ...reactHooks.configs.recommended.rules,
      'react/jsx-no-target-blank': 'off',
      'react-refresh/only-export-components': [
        'warn',
        { allowConstantExport: true },
      ],
    },
  },
]
```

### index.html
html
```
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="/vite.svg" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>RNM Auth</title>
  </head>
  <body>
    <div id="root"></div>
    <script type="module" src="/src/main.jsx"></script>
  </body>
</html>
```

### postcss.config.js
js
```
export default {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}
```

### vite.config.js
js
```
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'

// https://vite.dev/config/
export default defineConfig({
  plugins: [react()],
})
```

### tailwind.config.js
js
```
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### SERVER FOLDER CONTAINS :-
```
```
### index.js
import express from 'express'

const app = express()
```
![frontend design](https://github.com/user-attachments/assets/85d595b9-4890-413e-ae7d-0cc6dbaf4b05)
```
app.listen(3000,() => {
    console.log("Server is running")
})
```
