# react-native-swipeable-view-stack [![NPM version](https://badge.fury.io/js/react-native-swipeable-view-stack.svg)](https://npmjs.org/package/react-native-swipeable-view-stack) [![Build Status](https://travis-ci.org/Rajat%20Soni/react-native-swipeable-view-stack.svg?branch=master)](https://travis-ci.org/Rajat%20Soni/react-native-swipeable-view-stack)

> This is an interactive swipeable view stack npm package. Users can pan left or right on the frontmost view to naviagte to the next view. Data set is looped by defaut.

## Swipeable View Stack for React Native
![Alt text](https://cdn-images-1.medium.com/max/1600/1*fZMcXULoOCSGl8qBrHoILw.gif "Swipeable View Stack")

## Installation

```sh
$ npm install --save react-native-swipeable-view-stack
```

## Import and Usage
1) Import
```js
var ReactNativeSwipeableViewStack = require('react-native-swipeable-view-stack');
reactNativeSwipeableViewStack();
```
2) Usage
```jsx
<ReactNativeSwipeableViewStack
  onSwipe={ this.onCardSwipe }
  initialSelectedIndex={ 1 }
  data={ this.dataArray }
  renderItem={ ( data ) => this.renderViewItem( data ) }
/>
```

## License

ISC © [Rajat Soni](https://www.npmjs.com/~rajatsoni)
