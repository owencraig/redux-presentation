# Redux: Let's get immutable


--
# What's Redux?
--
> "a predictable state container for JavaScript apps"
> - [redux.js.org](http://redux.js.org/)
--
> "Awesome" 
> - [Cabcharge Plus](https://plus.cabcharge.com)
--
An implementation of the Flux architecture
![Flux](https://facebook.github.io/flux/img/flux-simple-f8-diagram-1300w.png)
--
Small library with:
 - Single Application state
 - One way data Flow
 - Amazing Tooling
--
Three main concepts:
 - Store: The single source of truth for your application state
 - Actions: Events, raised in response to something happening in your application
 - Reducers: Pure, immutable functions working against the store in response to actions



--
# The importance of immutability
--

``` javascript
function mutableSetName (state, name) {
    state.name = arguments.name; 
    return state;
}
```
vs: 

``` javascript
function immutableSetName (state, name) {
    return Object.assign({}, state, { name });
}
```
--
 - Side effect free functions are really easy to test
 - Immutable functions are easy to reason about
 - Pure functions are repeatable
--
All of which help to...
--
Enable time travel


--
# Why?
--
Why Not? (It *is* shiny after all...)
-- 
As application size grows so does complexity
--
Large components are often SRP violators
--
Managing communication between lots of components can be a real pain
--
Testing...



--
# How does redux help?
--
Single Source of truth
--
Uni directional data Flow
--
Immutable data
--
Pure functions are dreamy


--
# Some Code
--
![React Logo](https://facebook.github.io/react/img/logo.svg)
--
![Angular 2 Logo](https://angular.io/resources/images/bios/shield-bio-placeholder.png)

Coming soon - Sorry!


--
# Tooling
--
- [Dev Tools Extension](http://zalmoxisus.github.io/redux-devtools-extension/)
- [Dev Tools](https://github.com/gaearon/redux-devtools)


--
# Resources
--
- [redux.js.org](http://redux.js.org/) - Documentation, examples, walkthroughs
- [Getting started with Redux](https://egghead.io/series/getting-started-with-redux) - Dan Abramov's 30 free egghead videos