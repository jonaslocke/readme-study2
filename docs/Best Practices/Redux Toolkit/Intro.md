---
title: Introduction
id: Intro
---

This will give a very brief idea of how to use redux toolkit in our project. For in-depth knowledge please visit [here](https://redux-toolkit.js.org/)

## What is Redux Toolkit ?

Redux Toolkit is a very popular javascript state management library. The Redux Toolkit package is intended to be the standard way to write Redux logic. You can also use redux toolkit query along with the state management (same work that react query does)

## Why Redux Toolkit and not Redux ?

Redux is the library on top of which Redux Toolkit works. It was originally created to help address three common concerns about Redux:

- "Configuring a Redux store is too complicated"
- "I have to add a lot of packages to get Redux to do anything useful"
- "Redux requires too much boilerplate code"s

Redux Toolkit also includes a powerful data fetching and caching capability "RTK Query". It's included in the package as a separate set of entry points. It's optional, but can eliminate the need to hand-write data fetching logic yourself.

## What do you need before starting ?

### Install required dependencies

Your project is generally configured with all the dependencies and you just need to run the below command to get it will install all the required packages

```bash
    pnpm install
```
But if you need for some project where its not already there, then you need to install below packages 

```bash
    pnpm install @reduxjs/toolkit react-redux
```