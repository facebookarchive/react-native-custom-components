# React Native Legacy Custom Components

This is a module for legacy "CustomComponents" to gracefully deprecate.

## Navigator

The navigator component in this module will behave identically as the one in old version of React native, with one exception:

Latest documentation is available here: http://facebook.github.io/react-native/releases/0.43/docs/navigator.html


### Breaking Changes from react-native

- Navigator.props.sceneStyle must be a plain object, not a stylesheet!

(this breaking change is needed to avoid calling React Native's private APIs)

### Usage

Simply replace Navigator imports with the one from this package.

```js
import { Navigator } from 'react-native-deprecated-custom-components';
```

## NavigationExperimental

The NavigationExperimental module will behave identically as the one in React Native 0.43.

### Usage

Simply replace NavigationExperimental imports with the one from this package.

```js
import { NavigationExperimental } from 'react-native-deprecated-custom-components';
```
