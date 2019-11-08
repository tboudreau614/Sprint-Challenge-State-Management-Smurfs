1. What problem does the context API help solve?

The React Context API is a method for a child component to easily access a value stored within a given parent component.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

Actions are essentially payloads full of information that provide your data from your app to your store. They are the main source of information for the store within your app.
 
A reducer is a function that takes the past state and an action and also returns the next state

Store is essentially a plain JS object which allows a given component to share state throughout the app.

Redux is a single source of truth, it means that the only way to change your data in UI is to dispatch redux action which will change state within redux reducer. And your React components will watch this reducer and if that reducer changes, then UI will change itself too. But never other way around, because Redux state is single source of truth.

3. What is the difference between Application state and Component state? When would be a good time to use one over the other?

Application state is global state and the component state is local state.

4. Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?

Redux Thunk is middleware which allows you to call `action-creators` which return a function instead as opposed to an action object.

5. What is your favorite state management system you've learned and this sprint? Please explain why!

Personally, I enjoy using context the most. The reason for this is simply that I find it to be more straightforward and easy!