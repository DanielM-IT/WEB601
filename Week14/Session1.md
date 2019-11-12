# Week 14: Session 1

Today we are continuing with redux.

We looked at the stages involved in Redux this mornign since several of us were a bit foggy on this.
They are:
<ol>
    Action Creation
    Action
    Dispatch
    Reducers
    State
</ol>

Our tutor used an insurance claim as an analogy to represent how Redux is used. For instance we have the customer who fills out the claim form which is the action and the filling out is the action creation. They then take the form into the representative at the insurance companies front desk and give it to them. This is the dispatch stage.

We paused here and looked at how this pertains to the actual code. These actions represent the form filling out.

const createPolicy = (name, amount) => {
    return {
        type: 'DELETE_POLICY',
        payload: {
            name,
            amount
        }
    }
}

const deletePolicy = (name) => {
    return {
        type: 'DELETE_POLICY',
        payload: name
    }
}


Next up are the reducers. These are functions designed to take the current state and an action and return the next state.

const claimsHistory = (oldListOfClaims = [], action) => {
  if(action.type === 'CREATE_CLAIM') {
    return [...oldListOfClaims, action.payload];
  }
  return oldListOfClaims;
};

// Accounting
const accounting = (bagOfMoney = 100, action) => {
  if(action.type === 'CREATE_CLAIM') {
    return bagOfMoney - action.payload.amountOfMoneyToCollect;
  } else if(action.type === 'CREATE_POLICY') {
    return bagOfMoney + action.payload.amount;
  }
  return bagOfMoney;
};

Followed by the store creation and dispatching of the actions and their state change to the store.

const store = createStore(ourDepartments);

store.dispatch(createPolicy('Alex',50));
store.dispatch(createPolicy('Bob',30));
