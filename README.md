# RecipeFlix
RecipeFlix is a recipe discovery app made by a small team in one week in October 2023 as part of the CodeClan Professional Software Development course.

![Screenshot from 2023-11-10 11-04-51](https://github.com/ben-counsell/RecipeFlix/assets/97848152/4bcdb0d6-0911-4dbf-8a15-f88648f06ac0)

## Installation Instructions

Installation Requirements:

- Node Package Manager
- MongoDB

Clone the repo and navigate to the server directory in the terminal. Use `npm i` to install dependencies. Then make sure mongod is running and use `npm run seeds` to seed the database. A list of generated users will appear; copy one of their IDs to the clipboard. Now `npm run server:dev` should get the server up and running.

Unfortunately user verification is not yet available, so we will need to "log in" by opening the project in an IDE or text editor. Navigate to `app.jsx` then paste the user ID into the loggedInUserId variable on line 15.

It will also be necessary to insert a Spoonacular API key (which are freely available <a href="https://spoonacular.com/food-api">here</a>) into the `apiKey.jsx` file in the Services directory, formatted as follows:

```
const apiKey = {'x-api-key':'your-api-key-here'}

export default apiKey
```

Finally, we can navigate to the client directory using the terminal and use `npm i` to install any remaining dependencies. Now `npm run dev` should get the project up and running. Ctrl-click the link to open the app in your browser.

## Features
Users can use the drop-down menu to filter recipes based on a variety of criteria:

![recipeFlixTour1](https://github.com/ben-counsell/RecipeFlix/assets/97848152/33bbeb06-23f9-41f5-95aa-d8dae60010ea)

<hr/>

Users can also set their dietary requirements which will apply across the site, only showing recipes which are relevant to them:

<br/>

![Screenshot from 2023-11-10 13-40-03](https://github.com/ben-counsell/RecipeFlix/assets/97848152/48093eb8-6d65-406b-ab2b-2aa23a220a99)

<hr/>

Users can view recipe details, ingredients, and cooking method. They can also add recipes to their favourites:

<br/>

![Screenshot from 2023-11-10 13-41-47](https://github.com/ben-counsell/RecipeFlix/assets/97848152/c766f64f-b628-4407-8aff-0bda962810d4)

<hr/>

Users can also use the search bar to search for particular keywords:

<br/>

![Screenshot from 2023-11-10 13-44-40](https://github.com/ben-counsell/RecipeFlix/assets/97848152/b840e196-97df-447d-93ac-175175c35c62)

<hr/>
