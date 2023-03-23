# Expo Router Example

Use [`expo-router`](https://expo.github.io/router) to build native navigation using files in the `app/` directory.

## 🚀 About This Repo

I've setup this repo to demonstrate an error I am having setting up React Native Skia Web in a project using Expo Router. Would appreciate any and all assistance!

## 📝 Steps To Reproduce

- `npx create-expo-app@latest with-router`
- setup _layout route
- installed global expo cli
- `expo install @shopify/react-native-skia`
- `yarn setup-skia-web`
- `expo doctor --fix-dependencies`

## ⚠️ The Error

```
ERROR in ./node_modules/expo-router/entry.js:12:12
Module not found: Can't resolve '..\..\app'
  10 |   typeof window === "undefined" ? React.Fragment : Head.Provider;
  11 |
> 12 | const ctx = require.context(process.env.EXPO_ROUTER_APP_ROOT);
     |            ^
  13 |
  14 | // Must be exported or Fast Refresh won't update the context
  15 | export function App() {

web compiled with 1 error and 1 warning
```
