# Recipe App Task

## A CRUD (Create, Read, Update, Delete) application to manage recipes, built with Node.js, Express.js, and Mongoose (MongoDB), following the MVC architecture.

### Features
Create a Recipe: Add a new recipe to the database.
Retrieve Recipes: Fetch all recipes or a specific recipe by ID.
Update a Recipe: Modify details of an existing recipe by ID.
Delete a Recipe: Remove a recipe from the database by ID.
### Tech Stack
Node.js: Backend runtime environment.
Express.js: Web framework for routing and handling HTTP requests.
Mongoose: ODM for MongoDB integration.
Postman: API testing and documentation.
## Project Structure
```
Copy code
Recipe App/
├── controllers/
│   └── recipeController.js  # Handles recipe-related logic
├── models/
│   └── recipe.js            # Mongoose schema and model for recipes
├── routes/
│   └── recipeRoutes.js      # API route definitions
├── utils/
│   └── config.js            # Environment variable configuration
├── .env                     # Environment variables (e.g., MongoDB URI, PORT)
├── app.js                   # Express app setup
├── server.js                # Starts the server
└── package.json             # Project metadata and dependencies

```

## API Endpoints

```

Method	|    Endpoint	  |         Description
POST	|  /api/recipes	  |  Create a new recipe
GET	    |  /api/recipes	  |  Retrieve all recipes
GET	by ID     | /api/recipes/:id | 	Retrieve a recipe 
PUT	by ID     | /api/recipes/:id | 	Update a recipe 
DELETE 	by ID	 |/api/recipes/:id |	Delete arecipe 

```


## Create Recipe

### request
```
{
    "title":"Chettinad Prawn Masala",
    "ingredient":"['Prawn','Tomato ','onion','garlic','ginger']",
    "instuction":"De vein and clean the prawns. In a pan, add some oil and allow the cinnamon and fennels seeds to roast. Once it turns light brown, add the onion and saute it . Add little salt at this stage for the onion to cook faster.",
    "time":"1 hour"
}
```

### response


```
{
    "title":"Chettinad Prawn Masala",
    "ingredient":"['Prawn','Tomato ','onion','garlic','ginger']",
    "instuction":"De vein and clean the prawns. In a pan, add some oil and allow the cinnamon and fennels seeds to roast. Once it turns light brown, add the onion and saute it . Add little salt at this stage for the onion to cook faster.",
    "time":"1 hour"
}
```