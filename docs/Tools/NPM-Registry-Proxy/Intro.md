---
sidebar_position: 1
description: Describes the main purpose of NPM Registry Proxy
title: Introduction
id: Intro
displayed_sidebar: npmRegistrySideBar
---

This will help you to publish your reusable components as a JS library on your local and domain server

## What is NPM Registry Proxy ?

This is similar to publishing our packages or libraries to npm from where we usually download our dependencies. But as it's a customised project related resources we will host this within VIMO servers making it private. Every npm, pnpm or yarn call will go through this proxy before hitting actual NPM registry ([NPM registry ](https://www.npmjs.com/) will only be hit if packages could not be found in our own proxy server).

## Why we need the NPM Registry Proxy ?

Our custom libraries (say common-app-component) are not following versioning and all the changes in master become default for all projects. Further any custom requirement could not be achieved for seperate projects. Hoisting it behind the proxy and hence maintaining versions can help in more wider use case of the libraries.

## What do you need before starting ?

### Install required dependencies

- [Node](https://nodejs.org/en) v >=16.19.0
- [pnpm](https://pnpm.io/) v >= 8.0.0
- [Git](https://git-scm.com/)
- Any terminal

### Install optional dependencies for MacOS

- [nvm](https://github.com/nvm-sh/nvm) v 0.39.x


### Install [Verdaccio](https://www.npmjs.com/package/verdaccio) v >= 5.26.2


:::note It is required to install verdaccio globally
In your terminal execute the following command:

```bash
pnpm install --location=global verdaccio
```
:::