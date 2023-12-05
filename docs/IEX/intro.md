---
sidebar_position: 1
description: Describes the main purpose of iex directory app
---

# IEX Project

This project is the UI project for the IEX Project.

## What do you need before starting ?

### Install required dependencies

- [Node](https://nodejs.org/en) v >=16.19.0
- [pnpm](https://pnpm.io/) v >= 8.0.0
- [Git](https://git-scm.com/)
- Any terminal

### Install optional dependencies for MacOS

- [nvm](https://github.com/nvm-sh/nvm) v 0.39.x

### Setting up SSH credentials

Please configure your SSH cedentials following this [guide](https://confluence.atlassian.com/bitbucketserver/ssh-user-keys-for-personal-use-776639793.html).

###Â Cloning this repo

Open your terminal and execute the following command in the desired directory.

```bash
git clone git@bitbucket.org:getinsured/iex.git
```

Once the repo is cloned. Open your terminal and navigate to the project by running the following command:

```bash
cd iex
```

### Install dependencies

In your terminal execute the following command:

```bash
pnpm install
```

## Start the project

Open a terminal and execute the following command:

```
pnpm run local
```

This will start two applications: this FE application and a local backend server containing some API mocks to enable rapid development.

## Storybook

This project uses [Storybook](https://storybook.js.org/docs/7.0/react/get-started/install) v7 to generate docs. To preview this documentation, open your terminal and run the following command:

```bash
pnpm run storybook
```

##Â Unit Tests

This project uses [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/) and [vitest](https://vitest.dev/) to perform unit tests.

Every file following the file name convention `<fileName>.test.tsx` will be executed in the test.

Open your terminal and execute

```bash
pnpm run test
```

## Git

This project uses [husky](https://typicode.github.io/husky/#/) to configure some pre commits. For this project, the unit tests are performed before commiting to git. If all unit tests pass, the commit is allowed, otherwise the commit is denied until unit tests are fixed.

## Format

This project is configured with prettier to format the code. Please make sure to configure your IDE to apply this format rules to this project.

## Backend Developers

The configuration for the endpoints can be updated in the following file: `config/app.json`.

If you want to modify some endpoint, please modify it as follows:

```diff
{
  "appConfig": {
    "localhost": {
+      "apiBaseUrl": "http://localhost:8082"
      "apiUrls": {
        "environment": "/environment-va",
        "searchpublishedProviders": "/ms-providermgmt/providers/search"
      }
    },
    // more configs
  },
}

```

You can point to your specific server by modifying the apiBaseUrl field inside of the localhost configuration.

After you point to your local api base url, you can start the application as follows:

Open a terminal and run

```bash
pnpm run local
```

This will load the apiConfig.localhost configuration.

After running this command, open a browser and navigate to [http://localhost:5173/providermgmt/published-providers](http://localhost:5173/providermgmt/published-providers)

## Git Pre Commit Hooks

This repository uses [husky](https://typicode.github.io/husky/#/) to ensure that all commits do not break the current functionality of the application.

When you commit your changes, husky will run the script in the `.husky/pre-commit` file. For this case, every time you make a commit, the script will:

- Run all unit tests
- Find and fix problems in JS files by using ESLint
- Build the application

If all previous steps are able to run successfully, the commit will proceed, otherwise, the commit will be aborted and you will need to check what went wrong, fix the code, and commit again..

### Configuring husky

Husky needs a valid .git folder to run, since this application is inside a monorepo, we need to go to the parent directory in which the .git directory is located and install it from there

package.json
```json
{
  "name": "provider-directory",
  // more configuration
  "scripts": {
    // more scripts
    "prepare": "cd .. && husky install web/.husky"
  },
  // more configuration
}
```

### Installing husky

Husky is installed automatically after running the command `pnpm install`. This is because we specified to install husky in the [prepare](https://docs.npmjs.com/cli/v9/using-npm/scripts#life-cycle-scripts) command.

### Precommit script

You can specify what actions need to be completed/ checked before commiting in the `.husky/pre-commit` file:

```
#!/usr/bin/env sh
. "$(dirname -- "$0")/_/husky.sh"

cd web
npm run test && npm run lint && npm run build

```
> âš ï¸ *IMPORTANT* âš ï¸
>
> Since this commit is executed from the directory which contains the .git directory,
> you need to navigate to this directory to be able to run the npm scripts. See that we are
> running the `cd web` command before executing the npm scripts
