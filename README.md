# Recipe Planner

[Live Site URL](https://your-website-url.com)

## Description

Recipe Planner is a web application that allows users to plan meals, create a shopping list, and explore new recipes. The application enables users to save recipes, generate meal plans, and automatically compile a shopping list based on the ingredients required for the planned meals. It integrates with external APIs to fetch detailed recipe information, making meal planning easy and convenient.

## Features

### 1. User Authentication
- **Registration and Login:** Users can create an account or log in to access the full features of the application.
- **JWT-based Authentication:** Securely manages user sessions using JSON Web Tokens.

### 2. Recipe Management
- **Search for Recipes:** Users can search for recipes through an external API.
- **Save and Remove Recipes:** Users can save their favorite recipes to their accounts and remove them if needed. This feature provides a convenient way for users to organize recipes they want to use.
- **View Recipe Details:** Users can view detailed information about each recipe, including ingredients and instructions.

### 3. Meal Planning
- **Create Meal Plans:** Users can add saved recipes to their meal plans for each day of the week. This allows users to plan their meals efficiently.
- **Generate Shopping List:** Automatically generate a shopping list based on the ingredients of the recipes added to the meal plan.
- **Clear Shopping List:** Users have the option to clear the shopping list as needed.

### 4. User Flow
- **Login/Sign-Up:** New users can sign up for an account, while returning users can log in.
- **Save Recipes:** Users search for recipes, save their favorites, and later view or remove them.
- **Plan Meals:** Users add saved recipes to their meal plan for specific days and meal types (breakfast, lunch, dinner).
- **Generate Shopping List:** Based on the meal plan, users can generate and manage their shopping list.
- **Explore Random Recipes:** Users can explore random recipes for new meal ideas.


Ensure you have the necessary environment set up for the frontend.

## Standard User Flow

1. **Sign Up/Login:** The user creates an account or logs into the application.
2. **Explore Recipes:** The user can browse through random recipes or use the search functionality to find new recipes.
3. **Save Recipes:** The user saves recipes they want to try and can view these recipes in their "Saved Recipes" section.
4. **Plan Meals:** Using the "Meal Planner," the user adds selected recipes to their meal plan for specific days and meal types.
5. **Generate Shopping List:** The user generates a shopping list based on the ingredients needed for their meal plan.
6. **Manage Shopping List:** The user can check off items on the shopping list or clear the entire list when needed.

## API

### External API
- **Spoonacular API:** Used for fetching detailed recipe information, including ingredients and instructions.
- **API Documentation:** [Spoonacular API](https://spoonacular.com/food-api/docs)

### Custom API
- **Backend API:** The backend provides RESTful API endpoints to manage users, recipes, meal plans, and shopping lists.
- **Endpoints:**
  - `/auth/register` - Register a new user
  - `/auth/login` - Login and obtain a JWT token
  - `/recipes/save` - Save a recipe to the user's account
  - `/meal-plans` - Manage meal plans (create, fetch, delete)
  - `/shopping-list` - Manage the shopping list (fetch, clear)
- **Notes:** The backend API uses Express and PostgreSQL to store user data, recipes, meal plans, and shopping lists.

## Technology Stack

### Frontend
- **React:** For building the user interface.
- **React Router:** For managing navigation and routing.
- **Axios:** For making HTTP requests to the backend and external APIs.
- **Bootstrap:** For styling and responsive design.

### Backend
- **Node.js:** For building the server-side application.
- **Express:** For creating API endpoints.
- **PostgreSQL:** For storing user data, recipes, meal plans, and shopping lists.
- **JWT (JSON Web Token):** For user authentication and session management.

### Testing
- **Jest:** For running tests in both the frontend and backend.
- **Supertest:** For testing backend API endpoints.
- **React Testing Library:** For testing React components in the frontend.

### Hosting
- **Render:** The application is hosted using Render, which automatically deploys the app from GitHub branches.

## Important Notes
- **Environment Variables:** The application uses environment variables for API keys and database configuration. Make sure to set up your `.env` files for both frontend and backend correctly.
- **Project Structure:** The project is divided into two main directories:
- `frontend/` - Contains the React-based frontend application.
- `backend/` - Contains the Express-based backend application.

## Deployment
- **Frontend:** The frontend is set up to be deployed using the `npm run build` command to create a production build.
- **Backend:** The backend server is started using `node server.js`. For deployment, ensure that the environment variables for the database and API keys are properly configured.

## Future Enhancements
- Implement more advanced recipe search filtering.
- Introduce user profile management for dietary preferences.
- Add more tests to cover edge cases and improve the robustness of the application.



