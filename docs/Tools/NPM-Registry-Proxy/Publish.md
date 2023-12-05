---
sidebar_position: 1
description: Describes how to publish package to local server
title: Publish Package
id: PublishPackage
displayed_sidebar: npmRegistrySideBar
---

## Make changes to package

- Make some changes to library (here we have used common-app-component). 

:::note
These changes are intended only for testing the functionality of verdaccio and not meant to be pushed to the master of any repo. Any demo library can be used too for this purpose.
:::

- Change the package version to something higher to maintain versioning of the package. Package.json conatins the version of the package you are going to publish

- Move to the root directory of your package and open a terminal in it.
- Build your project using below command

```bash
pnpm run build
```

- Run the following command in the terminal

```bash
npm adduser --registry http://localhost:4873/
```
:::info
To publish a library we first have to authenticate using the command "npm adduser". Since the default registry is the NPM, the generated token will refer to that. We need to add the option --registry to define the registry the token refers to.
:::

- The command to publish the library is "npm publish". This however will publish the library into the NPM. Since we want to publish it in Verdaccio, we will add the option --registry in the command.

```bash
npm publish --registry http://localhost:4873/
```
- You just published your pacakge/library on your local server. Navigate to the local host address where verdaccio is running. You will be able to see your packaged published there.

![PUBLISHED PACKAGE](../../static/images/npm-registry/publishedPackage.png)

:::tip
If you are not able to publish your package try below troubleshot

- Make sure you have installed verdaccio globally
- Make sure your verdaccio server is running
- Make sure you are in the root directory of package and you have a valid package.json file
- Still not able to publish your package? Visit official [docs](https://verdaccio.org/docs/what-is-verdaccio) for in depth debug.
:::

## Publish newer version

Let's modify something more in the package/library we just published and this time make its version higher than the previuos one.

Run the below command again

```bash
npm publish --registry http://localhost:4873/
```

Check the UI and click on the published package and inside that navigate to versions tab. You should be able to see two different versions that we published

![Published Versions](../../static/images/npm-registry/publishedVersions.png)