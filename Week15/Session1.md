# Week 15: Session 1

This morning we are looking at how to wire Redux into our React components. To do this we will be following along with our tutor in building a basic book app which uses Redux to show books and change their state.

The below depiction gives and idea of the libraries. The libraries from both React and Redux are imported and then combined to manage the state within the application.

   React
    | ^
    v |
 React-redux
    | ^
    v |
   Redux

This small application is much like the ones we have done previously where we set up the store creator, create our action creators, reducers and dispatchers. These we then use to change state on our applications UI. In this case we are allowign the user to click on a specific book which will then retrieve its details from the database. The details include it title and notes. The reason for these two is that we will be using two reducers in this application and Redux only handles one. Thus we will be using a function called combineReducers() which allows the reducers to be combined and considered as one by Redux but still usable individually.

After completing this mini project for homework we have been asked to do a simple app project that starts with the state of a number at 0. We should then be able to increment or deincrement by 1. This project will use the combined react-redux that we used in class to make it work.