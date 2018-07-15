# react-native-swipeable-view-stack [![NPM version](https://badge.fury.io/js/react-native-swipeable-view-stack.svg)](https://npmjs.org/package/react-native-swipeable-view-stack) [![Build Status](https://travis-ci.org/Rajat%20Soni/react-native-swipeable-view-stack.svg?branch=master)](https://travis-ci.org/Rajat%20Soni/react-native-swipeable-view-stack)

> This is an interactive swipeable view stack npm package. Users can pan left or right on the frontmost view to naviagte to the next view. Data set is looped by defaut.

## Swipeable View Stack for React Native
![Alt text](https://cdn-images-1.medium.com/max/1600/1*fZMcXULoOCSGl8qBrHoILw.gif "Swipeable View Stack")

## Installation

```sh
$ npm install --save react-native-swipeable-view-stack
```

## Import and Basic Usage
1) Import
```js
var ReactNativeSwipeableViewStack = require('react-native-swipeable-view-stack');
reactNativeSwipeableViewStack();
```
2) Basic Usage
```jsx
<ReactNativeSwipeableViewStack
  onSwipe={ this.onCardSwipe }
  initialSelectedIndex={ 1 }
  data={ this.dataArray }
  renderItem={ ( data ) => this.renderViewItem( data ) }
/>
```

## Props
__onSwipe( swipedIndex: number )__: (Optional) Gets called when navigation is about to take place.
__initialSelectedIndex: number__: (Optional) Element at index to be shown at the top of the stack initially.
__stackSpacing: number__: (Optional) Top spacing between stacked views.
__data: Array__: Array of Elements that'll be represented by this component.
__onItemClicked: Function__: Inputs a function and gets called when the frontmost card is clicked.
__renderItem: Function__: Inputs a function that returns view items of stack.

## License

ISC © [Rajat Soni](https://www.npmjs.com/~rajatsoni)
