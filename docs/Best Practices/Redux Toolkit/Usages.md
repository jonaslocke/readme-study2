---
title: Usage and Configuration
id: usage
---

## Configuration
A quick overview how redux toolkit is configured. For detailed setup and options please visit [here](https://redux-toolkit.js.org/tutorials/quick-start)
 ### 1. Configure Store

```ts
  ...
   export const store = configureStore({
        reducer: {
            usersCombinedReducer,
            appConfig,
            [getEnv.reducerPath]: getEnv.reducer
        },
        middleware: (getDefaultMiddleware) => getDefaultMiddleware().concat([getEnv.middleware]).concat(logger)
    });

    export type RootState = ReturnType<typeof store.getState>;

    export type AppDispatch = typeof store.dispatch;
    ...
```

### 2. Wrap Parent With Store

```tsx
  .....
    <Provider store={store}>
      .....
      <RouterProvider router={router} />
      .....
    </Provider>
    .....
```

### 3. Using the state in component

```tsx
  .....
      const users = useAppSelector((state) => state.usersCombinedReducer.users);
      const envUrl = useAppSelector(baseUrl) + '/environment';
      const dispatch = useAppDispatch();
      .....
      const addUser = (formdata) => {
            dispatch(addUserAction(formdata));
      };
    .....
```

### 4. Using RTK to call api

```tsx
  ..... 
  //endpoint setup
    export const getEnv = createApi({
        reducerPath: 'getEnv',
        baseQuery: fetchBaseQuery({ baseUrl: '' }),
        endpoints: (builder) => ({
            env: builder.query({
                query: (url: string) => url
            })
        })
    });

export const { useEnvQuery } = getEnv;
 //you must add the endpoint as a middleware in store creation
    .....

    //calling the api
    const data = useEnvQuery(envUrl);
    console.warn('using RTK', data);
```
### Redux Devtool
Add the [Redux devtool](https://chromewebstore.google.com/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd) extension to your browser to see state in a visual graph 

### Note: 
Go through the [official](https://redux-toolkit.js.org/) docs of redux toolkit for more in depth configs and apis available