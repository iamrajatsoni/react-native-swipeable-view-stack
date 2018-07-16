# react-native-swipeable-view-stack [![NPM version](https://badge.fury.io/js/react-native-swipeable-view-stack.svg)](https://npmjs.org/package/react-native-swipeable-view-stack) [![Build Status](https://travis-ci.org/Rajat%20Soni/react-native-swipeable-view-stack.svg?branch=master)](https://travis-ci.org/Rajat%20Soni/react-native-swipeable-view-stack)

> This is an interactive swipeable view stack npm package. Users can pan left or right on the frontmost view to naviagte to the next view. Data set is looped by defaut.

## Swipeable View Stack for React Native
![Alt text](https://cdn-images-1.medium.com/max/1600/1*fZMcXULoOCSGl8qBrHoILw.gif "Swipeable View Stack")

## Installation

```sh
$ npm install --save react-native-swipeable-view-stack
```

## Import and Basic Usage
__Import__
```js
var ReactNativeSwipeableViewStack = require('react-native-swipeable-view-stack');
reactNativeSwipeableViewStack();
```
__Basic Usage__
```jsx
<ReactNativeSwipeableViewStack
  onSwipe={ ( swipedIndex ) => this.onCardSwipe( swipedIndex ) }
  initialSelectedIndex={ 1 }
  data={ this.dataArray }
  renderItem={ ( element ) => this.renderViewItem( element ) }
  onItemClicked={ ( element ) => this.onClick( element ) }
  stackSpacing={ 20 }
/>
```

## Props
* __onSwipe( swipedIndex: number )__: (Optional) Gets called when navigation is about to take place.

* __initialSelectedIndex: number__: (Optional) Element at index to be shown at the top of the stack initially.

* __stackSpacing: number__: (Optional) Top spacing between stacked views.

* __data: Array__: Array of Elements that'll be represented by this component.

* __onItemClicked( element: ~Clicked Element ): Function__: Function to be executed when the frontmost card is clicked.

* __renderItem( element: ~Array Element): Function__: Inputs a function that returns view items of stack.

## Important Note
\*\*\* You have to specify the __width__ & __height__ of __renderItem__ view, otherwise you might see unusual behaviour.


## License

ISC © [Rajat Soni](https://www.npmjs.com/~rajatsoni)
