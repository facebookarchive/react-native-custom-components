# React Native Legacy Custom Components

This is a module for legacy "CustomComponents" to gracefully deprecate.

## Navigator

The navigator component in this module will behave identically as the one in old version of React native, with one exception:

Latest documentation is available here: http://facebook.github.io/react-native/releases/0.43/docs/navigator.html


### Breaking Changes from react-native

- Navigator.props.sceneStyle must be a plain object, not a stylesheet!

(this breaking change is needed to avoid calling React Native's private APIs)

### How to use it

Example use of `Navigator`

```
import React, {Component} from 'react';
import { AppRegistry, StyleSheet, View } from 'react-native';

import CustomComponents from 'react-native-deprecated-custom-components';

export default class ExampleApp extends Component {

  render() {
    return (
      <View style={styles.container}>

        <CustomComponents.Navigator />

      </View>
    );
  }

}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#eeeeee',
  },
});

AppRegistry.registerComponent('ExampleApp', () => ExampleApp);
```
