---
sidebar_position: 1
description: Describes how to start local server
title: Setup Local Server
id: SetupLocalServer
displayed_sidebar: npmRegistrySideBar
---

## Start the Verdaccio server

In your terminal execute the following command:

```bash
verdaccio
```
:::info 
Your server should start on [port](http://localhost:4873/) http://localhost:4873/ by default.
Visiting the address should show empty registry as we have not pushed anything.
:::


If everything is ok you will be able to see verdaccio homepage like below

![Homepage Verdaccio](../../static/images//npm-registry/verdaccio-home.png)

Now your local server is up and running. Now lets publish some package to the registry