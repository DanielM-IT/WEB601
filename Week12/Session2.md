With another classes assignment deadline upon me I have not done anything but what is done in class today.  
In this session we have been given freecodecamp exercises to do all class. These are based upon Redux which is our next topic we are moving into. Redux allows us to take an objects state, execute an action on it and provide a new state out of it.

Below are some of the things learned through freecodecamp:

### Creating the store which contains an applications state

const store = Redux.createStore(reducer)

### Creating actions which are later performed to change the state

let action = {
    type: 'LOGIN'
}

### Using the dispatch function to dispatch actions to the store

store.dispatch(loginAction())

### Using and combining reducers which specify how the applications state changes when actions are sent to the store

const rootReducer = Redux.combineReducers({
  count: counterReducer,
  auth: authReducer
})

Each week a group of 5 of us will be going to a company called "Shuttlerock" to visit, have a look around and ask questions. I went with the first group after this afternoons session. The intention behind these visits is to give us a feel for the work environment of a developer and ask questions that will better help us understand what we can expect.
