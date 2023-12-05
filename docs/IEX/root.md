---
sidebar_position: 3
description: Describes the main purpose of provider directory app
---

# Root

The file located under src/routes/root.tsx is basically the main entry React page and the layout of the app.
This React component is responsible for fetching the token, get the environment information and load the correct translation bundle.

This component is wrapped by a component named Auth.

<!-- ## Auth

This component wraps to the root component. It is responsible to get the token from the following endpoint: `/hix/account/user/token`.
Once the token is fetched, it is stored on the session storage. -->

<!-- ## Environment 

The root component fetches the environment from the following endpoint: `/providermgmt/providers/environment`. Once is fetched, the environment is stored on the `src/modules/provider-management/hooks/useEnvironmentStore.tsx` hook and can be accessed across the entire app.

More info: [Zustand](https://github.com/pmndrs/zustand)

## Translation bundle

Once the environment is fetched, the translation bundle is loaded for the correct state. The state code comes in the environment object in the `environment.configuration.stateCode` property. -->