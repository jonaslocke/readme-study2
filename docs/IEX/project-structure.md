---
sidebar_position: 1
description: Describes the main purpose of provider directory app
---

# Project Structure

This project has the following structure:

```
.
├── README.md
├── mocks
│   ├── index.json
├── config
│   ├── env,js
│   ├── paths.js
│   ├── polyfills.js
│   └── webpack.config.prod.js
├── jest.setup.js
├── jest.config.js
├── postcss.config.js
├── enzyme.js
├── package.json
├── pnpm-lock.yaml
├── public
│   └── index.html
├── src
│   ├── actions
│   ├── APIs
│   ├── components
│   ├── configs
│   ├── constants
│   ├── containers
│   ├── contexts
│   ├── routes
│   ├── hooks
│   ├── i18n
│   ├── lib
│   ├── modules
│   ├── reducers
│   ├── routes
│   ├── sages
│   ├── selectors
│   ├── services
│   ├── store
│   ├── test-utils
│   ├── utils
│   ├── index.html
│   └── index.js
├── assets
├── tsconfig.json
└── webpack.config.js
```

## README.md (file)

This file contains the necessary information to run the project.

## config (dir)

Contains the global configuration for the app

## config/app.json (file)

Contains the global configurations for the app. In this file we have defined information like:

- Backend Endpoint URLS
- Tokens
- Configurations for specific pages

Do you want to add a new backend endpoint? This is the correct place.
This config file is used and loaded by the useAppConfig hook.

## i18n (dir)

Contains the translations json files for the project.
Do you want to add a new translation? Modify it ? This is the correct place

## uploadProvidersConfig.json (file)

Contains the configuration for the Process Status page (Step 2) of the Upload Provider Data page.

## index.html (file)

This is the entry file of the app
More info? Visit [Vite](https://vitejs.dev/guide/#index-html-and-project-root)

## jest.config.ts (file)

Contains the configuration for jest.

## migration-storybook.log (file)

Storybook migration log
More info: [Storybook](https://storybook.js.org)

## package.json (file)

Heart of node project
More info: [package.json](https://docs.npmjs.com/cli/v9/configuring-npm/package-json)

## pnpm-lock.yaml (file)

Metadata about packages
[pnpm](https://pnpm.io/cli/install)

## public (dir)

Public static asset directory of vite
More info [Static Asset Handling]https://vitejs.dev/guide/assets.html

## src (dir)

Contains all the interesting stuff of the project. In this directory you find basically all the code

### assets

Contains the static assets of this app

### core/components

Contains the shared and reusable components for this app.

### core/network

Contains the code of our custom http client. It uses axios behind the scenes.

### core/pdf

Contains the common configuration for PDF creation. It uses pdfMake behind the scenes.

### hooks

Contains the shared hooks for this app.

### main.tsx

Main entry file for this app

### modules

Contains all the pages and components for this app.

### routes

Contains the configuration for the route definition.

### shared

Contains code that is shared across multiple pages

### tests/utils

Contains the confiration of react testing library that can be used to test all components.
More info [Setting up RTL](https://testing-library.com/docs/react-testing-library/setup/)


