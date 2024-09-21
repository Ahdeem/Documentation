# Recipe API Documentation

**Version:** 1.0  
**Git Project URL:** `https://github.com/bernardAppah/recipeApi`

## Introduction
The Recipe API platform provides a set of endpoints for registered users to manage and explore recipes. Users can add new recipes, filter recipes based on various criteria, update existing recipes, and delete recipes.

This documentation is intended for developers who want to integrate recipe management capabilities into their applications.

## Endpoints
1. Register a user
   - EndPoint: /api/recipe/register-user
   - Method: POST
   - Parameters: There are two required parameters: Name and Password
   - Description: Creates a new user account to access the recipe API
   - Response:
     + Scenario 1: Unique username:
       ![Scenario1](./RegisteredUser1.jpg)

     + Scenario 2: When an existing username is provided:
       ![Scenario2](./RegisteredUser2.jpg)

2. Add a new recipe
    - EndPoint: /api/recipe/add-recipe
    - Method: POST
    - Parameters: Only one parameter is required and that is the userId
    - Description: Creates a new recipe as entered by a registered user.
    - Request:
        ![SampleRequest](./AddRecipeRequestHappyFlow.jpg)
    - Response:
        + Scenario 1 : Attempt to create a recipe with a registered user
          ![HappyFlow](./AddRecipeResponseHappy.jpg)
        + + Scenario 2 : Attempt to create a recipe with an uregistered user
          ![NonHappyFlow](./AddRecipeResponseNonHappy.jpg)

3. Delete Recipe

```

```

