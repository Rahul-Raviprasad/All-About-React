# Redux

A predictable state container for javascript apps

https://github.com/reactjs/redux

This is not specific to the browser or the server, although it tends to incline towards the browser. It is mostly agnostic to the environment.

## Why Redux?
Took from the facebooks flux architecture
So flux is basically NIH event emitter with event ordering?

so redux is a take on the same thing but is considered to be simpler.

It was unveiled by Dan Abramov at react-europe 2015

## Main ideas of Redux
* Single source of truth
* Uni directional data flow
* Read only state
* enforces immutability
* Composable
* Its all just functions

## the pattern

State  -----> view
  \           /
    \       /
     update
