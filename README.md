# 18-unit

# Recipe App with React

## Instructions

Follow the steps below to build your recipe application. 

1. Use create-react-app to create a new application. 
2. Create a stateful component called `App`. 
3. Add an array of objects to the state.
4. Create a component called `DirectoryView`. This component will render the search form and the recipe cards. 
5. Create a component called `SearchForm` that renders an input box and a search button. 
6. Create a component called `RecipeCard` that renders a div with the word 'recipe name'. 
7. `DirectoryView` should render `SearchForm` and `RecipeCard`. `App` should render `DirectoryView`. 
8. Pass the recipe list from state to `DirectoryView`. 
9. In `DirectoryView`, map over the recipe list and render one recipe card for each recipe in the list. 
10. In `DirectoryView`, pass the name of each recipe to the `RecipeCard` component inside your map function. 
11. `RecipeCard` should render the recipe name passed to it. 
12. In `App` create a new property on state called `searchVal`.
13. In `App` create a function called `handleChange` that takes a paremeter called `event` and updates the `searchVal` property to `event.target.value`.
14. In `App`, pass the `handleChange` function and `searchVal`  to `DirectoryView`.
15. In `DirectoryView`, pass the `handleChange` function and `searchVal` to `SearchForm`
16. In `SearchForm`, add a change listener to the input field that calls the `handleChange` function every time the input field changes.
17. In `SearchForm`, add a `value` attribute to the input that equals the `searchVal`
18. In `App`, create a new property on state called `selectedRecipes`. 
19. In `App`, create a function called `selectRecipes`. This function takes in no paremeters. When this function executes it should use filter to create a new array that has every object from the original recipe list whose name includes the `searchVal`, then update `selectedRecipes` to this new array.
20. In `App`, pass the `selectRecipes` function to `DirectoryView`.
21. In `DirectoryView`, pass the `selectRecipes` function to `SearchForm`.
22. In `SearchForm`, add a click listener to the button that triggers the `selectRecipes` function when the button is clicked. 
23. Alter `App` to pass `selectedRecipes` to `DirectoryView` instead of the full recipe list. 
24. Create a new component called `DetailView`. 
25. In `App` render `DetailView` and pass it the first object in the recipe list. 
26. In `DetailView` render the name, ingredients, and instructions for the recipe. 
27. When a user clicks on a recipe in the `DirectoryView`, update the `DetailView` to show the details for that recipe.
