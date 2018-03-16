# FAQ

## Table of Contents

* **General**
  * [When should I learn Redux?](general.md#general-when-to-learn)
  * [When should I use Redux?](general.md#general-when-to-use)
  * [Can Redux only be used with React?](general.md#general-only-react)
  * [Do I need to have a particular build tool to use Redux?](general.md#general-build-tools)
* **Reducers**
  * [How do I share state between two reducers? Do I have to use combineReducers?](reducers.md#reducers-share-state)
  * [Do I have to use the switch statement to handle actions?](reducers.md#reducers-use-switch)
* **Organizing State**
  * [Do I have to put all my state into Redux? Should I ever use React's setState\(\)?](organizing-state.md#organizing-state-only-redux-state)
  * [Can I put functions, promises, or other non-serializable items in my store state?](organizing-state.md#organizing-state-non-serializable)
  * [How do I organize nested or duplicate data in my state?](organizing-state.md#organizing-state-nested-data)
* **Store Setup**
  * [Can or should I create multiple stores? Can I import my store directly, and use it in components myself?](store-setup.md#store-setup-multiple-stores)
  * [Is it OK to have more than one middleware chain in my store enhancer? What is the difference between next and dispatch in a middleware function?](store-setup.md#store-setup-middleware-chains)
  * [How do I subscribe to only a portion of the state? Can I get the dispatched action as part of the subscription?](store-setup.md#store-setup-subscriptions)
* **Actions**
  * [Why should type be a string, or at least serializable? Why should my action types be constants?](actions.md#actions-string-constants)
  * [Is there always a one-to-one mapping between reducers and actions?](actions.md#actions-reducer-mappings)
  * [How can I represent “side effects” such as AJAX calls? Why do we need things like “action creators”, “thunks”, and “middleware” to do async behavior?](actions.md#actions-side-effects)
  * [Should I dispatch multiple actions in a row from one action creator?](actions.md#actions-multiple-actions)
* **Immutable Data**
  * [What are the benefits of Immutability?](immutable-data.md#benefits-of-immutability)
  * [Why is immutability required in Redux?](immutable-data.md#why-is-immutability-required)
  * [Do I have to use Immutable.JS?](immutable-data.md#do-i-have-to-use-immutable-js)
  * [What are the issues with using ES6 for immutable operations?](immutable-data.md#issues-with-es6-for-immutable-ops)
* **Using Immutable.JS with Redux**
  * [Why should I use an immutable-focused library such as Immutable.JS?](../recipes/using-immutable.js-with-redux.md#why-use-immutable-library)
  * [Why should I choose Immutable.JS as an immutable library?](../recipes/using-immutable.js-with-redux.md#why-choose-immutable-js)
  * [What are the issues with using Immutable.JS?](../recipes/using-immutable.js-with-redux.md#issues-with-immutable-js)
  * [Is Immutable.JS worth the effort?](../recipes/using-immutable.js-with-redux.md#is-immutable-js-worth-effort)
  * [What are some opinionated Best Practices for using Immutable.JS with Redux?](../recipes/using-immutable.js-with-redux.md#immutable-js-best-practices)
* **Code Structure**
  * [What should my file structure look like? How should I group my action creators and reducers in my project? Where should my selectors go?](code-structure.md#structure-file-structure)
  * [How should I split my logic between reducers and action creators? Where should my “business logic” go?](code-structure.md#structure-business-logic)
  * [Why should I use action creators?](code-structure.md#structure-action-creators)
* **Performance**
  * [How well does Redux “scale” in terms of performance and architecture?](performance.md#performance-scaling)
  * [Won't calling “all my reducers” for each action be slow?](performance.md#performance-all-reducers)
  * [Do I have to deep-clone my state in a reducer? Isn't copying my state going to be slow?](performance.md#performance-clone-state)
  * [How can I reduce the number of store update events?](performance.md#performance-update-events)
  * [Will having “one state tree” cause memory problems? Will dispatching many actions take up memory?](performance.md#performance-state-memory)
  * [Will caching remote data cause memory problems?](performance.md#performance-cache-memory)
* **Design Decisions**
  * [Why doesn't Redux pass the state and action to subscribers?](design-decisions.md#does-not-pass-state-action-to-subscribers) 
  * [Why doesn't Redux support using classes for actions and reducers?](design-decisions.md#does-not-support-classes) 
  * [Why does the middleware signature use currying?](design-decisions.md#why-currying)
  * [Why does applyMiddleware use a closure for dispatch?](design-decisions.md#closure-dispatch)
  * [Why doesn't `combineReducers` include a third argument with the entire state when it calls each reducer?](design-decisions.md#combineReducers-limitations)
  * [Why doesn't `mapDispatchToProps` allow use of return values from `getState()` or `mapStateToProps()`?](design-decisions.md#no-asynch-in-mapDispatchToProps)
* **React Redux**
  * [Why isn't my component re-rendering, or my mapStateToProps running?](react-redux.md#react-not-rerendering)
  * [Why is my component re-rendering too often?](react-redux.md#react-rendering-too-often)
  * [How can I speed up my mapStateToProps?](react-redux.md#react-mapstate-speed)
  * [Why don't I have this.props.dispatch available in my connected component?](react-redux.md#react-props-dispatch)
  * [Should I only connect my top component, or can I connect multiple components in my tree?](react-redux.md#react-multiple-components)
* **Miscellaneous**
  * [Are there any larger, “real” Redux projects?](miscellaneous.md#miscellaneous-real-projects)
  * [How can I implement authentication in Redux?](miscellaneous.md#miscellaneous-authentication)

