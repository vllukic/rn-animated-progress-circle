# React Native Animated Progress Circle

### Props

| PROP                    | TYPE      | DESCRIPTION                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ----------------------- | --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| percent                 | Number    | Number between `0-1` which indicates the total progress. Default percent is `0`.                                                                                                                                                                                                                                                                                                                                              |
| size                    | Number    | Sets the size of the progress circle. Default size is `64`.                                                                                                                                                                                                                                                                                                                                                                   |
| thickness               | Number    | Sets the thickness of the progress circle. Default thickness is `7`                                                                                                                                                                                                                                                                                                                                                           |
| color                   | String    | Sets the color of the complete portion of the progress circle. Default color is `#7e42ed`.                                                                                                                                                                                                                                                                                                                                    |
| unfilledColor           | String    | Sets the color of the incomplete portion of the progress circle. Default unfilledColor is `transparent`.                                                                                                                                                                                                                                                                                                                      |
| style                   | Object    | Any arbitrary styles you want to pass to the component.                                                                                                                                                                                                                                                                                                                                                                       |
| children                | ReactNode | Any children you want to appear in the center of the progress circle.                                                                                                                                                                                                                                                                                                                                                         |
| animationMethod         | String    | Animation method to be used. Takes one of the following strings: `timing`, `spring`, `bounce`, `decay`. Setting this value will animate the component.                                                                                                                                                                                                                                                                        |
| animationConfig         | Object    | Configuration object to set animation parameters. See configuration docs for [timing](https://facebook.github.io/react-native/docs/animated#timing), [spring](https://facebook.github.io/react-native/docs/animated#spring), [bounce](https://facebook.github.io/react-native/docs/animated#bounce), and [decay](https://facebook.github.io/react-native/docs/animated#decay). `useNativeDriver` is set to `true` by default. |
| shouldAnimateFirstValue | Boolean   | Indicates whether the initial value passed to the `percent` prop should animate in or not. Defaults to `false`. If set to true, the animation method used is `timing` and the default configuration is `{ duration: 200 }`, unless otherwise specified via `animationMethod` and `animationConfig` props.                                                                                                                     |
| onChange                | Function  | Callback function which gets called when the `percent` prop changes.                                                                                                                                                                                                                                                                                                                                                          |
| onChangeAnimationEnd    | Function  | Callback function which gets called when the animation that occurs after the `percent` prop changes is complete.                                                                                                                                                                                                                                                                                                              |

### Examples

#### Animated.spring to animate value changes with Text as children

![animated gif of progress circle changing to different percentages of completion](https://raw.githubusercontent.com/simonsteer/rn-animated-progress-circle/master/examples/animated-spring.gif)

[source](https://github.com/simonsteer/rn-animated-progress-circle/blob/master/examples/AnimatedSpring.js)

#### Recreation of the native Android spinner

![animated gif of native android spinner](https://raw.githubusercontent.com/simonsteer/rn-animated-progress-circle/master/examples/android-spinner.gif)

[source](https://github.com/simonsteer/rn-animated-progress-circle/blob/master/examples/AndroidSpinner.js)
