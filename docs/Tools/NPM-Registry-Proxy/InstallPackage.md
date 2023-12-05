---
sidebar_position: 1
description: Describes how to install package from local server
title: Install Package
id: InstallPackage
displayed_sidebar: npmRegistrySideBar
---

## Install published package

To install any package we use npm or pnpm or yarn. So let's run the below command

:::note
Before running below command follow the steps

- Move to any project where you want to install the published package
- Remove the previously installed @getinsured/common-app-components from package.json (for cleaner install)
:::

```bash
pnpm install @getinsured/common-app-components
```

:::caution
Above command will fail since we haven't published our package into NPM, rather its still in our local server.
:::

### Add .npmrc file

To overcome the above error faced we need to add a file .npmrc in route directory of the project where you are trying install the package.

- Add the file .npmrc to root directory
- Add below lines in the .npmrc file

```bash
registry=http://localhost:4873
```

:::info
Adding the above file and registry value equal to our server address, let's npm or yarn or pnpm to look for the packages in our local server and if thats not found then only it goes through normal process of installing from npmjs. So it creates a proxy through which all install command passes.
:::

## Install published package again

Now let's try again and run the below command

```bash
pnpm install @getinsured/common-app-components
```

This should install the latest package from the local server. Verify the version installed.

### Install specific version

Now we might need to install specific version of the package as per project usage. So let's try installing the lower version 

Run the below command

```bash
pnpm install @getinsured/common-app-components@0.0.30
```
:::note
Use the same package name and version as you published. Above command uses package version and name as per this document
:::

This will install the package with version v0.0.30. Verify your package.json file if correct version got downloaded

:::tip
If your installation fails, try with below steps

- Make sure your local server of verdaccio is up and running
- Make sure you have correctly given your package name and version
- Try restarting the verdaccio server
:::