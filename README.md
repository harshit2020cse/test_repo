# react-native-app-compat-components
A lightweight View component that can be styled quickly.

Installation
---
```javascript
$ npm install react-native-app-compat-components
```
then
```javascript
import { AppCompatView } from 'react-native-app-compat-components';
/*...*/
<AppCompatView enableBottomSafeArea={false}>
/*...*/
</AppCompatView>
```

or
```javascript
import { AppCompatScrollView } from 'react-native-app-compat-components';
/*...*/
<AppCompatScrollView>
/*...*/
</AppCompatScrollView>
```

## API

### AppCompatView

You need to direcly import the AppCompatView in your class/function.

#### Example

```js
import { AppComaptView } from 'react-native-app-compat-components';

function App() {
  return <AppComaptView enableBottomSafeArea={true}><View>...</View></AppComaptView>;
}
```
#### Props

Accepts all [View](https://reactnative.dev/docs/view#props) props. Has a default style of `{flex: 1}`.

##### `enableTopSafeArea`

Optional, defaults to `true`.

Can be used to provide the initial value for frame and insets, this allows rendering the view with preventing from top safe area.

##### `enableBottomSafeArea`

Optional, defaults to `true`.

Can be used to provide the initial value for frame and insets, this allows rendering the view with preventing from bottom safe area.

##### `rootContainerStyle`

Can be used to provide the custom style to the root container view which inclueds safe area.

##### `innerViewStyle`

Can be used to provide the custom style to the inner view.

##### `children`

Can be used to provide any view, It accepts single of multiple views.

### AppCompatScrollView

You need to direcly import the AppCompatScrollView in your class/function.

#### Example

```js
import { AppComaptScrollView } from 'react-native-app-compat-components';

function App() {
  return <AppComaptScrollView><Text></Text><View>...</View></AppComaptScrollView>;
}
```
#### Props

Accepts all [View](https://reactnative.dev/docs/view#props) props. Has a default style of `{flex: 1}`.

##### `rootContainerStyle`

Can be used to provide the custom style to the root container view which inclueds safe area.

##### `scrollViewStyle`

Can be used to provide the custom style to the scroll view.

##### `innerViewStyle`

Can be used to provide the custom style to the inner view.

##### `children`

Can be used to provide any view, It accepts single of multiple views.
