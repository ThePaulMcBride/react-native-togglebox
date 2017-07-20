# react-native-togglebox
React Native Toggle Box for showing/hiding content with sliding effect. Should looks like classical [slideToggle()](http://api.jquery.com/slidetoggle/) from jQuery.

* The `ToggleBox` scene should be wrapped in a `ScrollView` to allow the page to grow as the toggle opens
* PRs welcome

## Demo

![Showtime](.github/react-native-show-hide-toggle-box.gif?raw=true "Showtime")

## Installation

```bash
npm i react-native-togglebox --save
```

or

```bash
yarn add react-native-togglebox --save
```

## Use

```javascript
import ToggleBox from 'react-native-show-hide-toggle-box'

...

<ScrollView style={styles.container}>
  <ToggleBox label='Toggle this box' value='Tap Me' style={{backgroundColor: '#ddd', borderBottomWidth: 1}}>
    <View style={{height: 300, alignItems: 'center', justifyContent: 'center', backgroundColor: '#eee'}}>
      <Text>Hello, world!</Text>
    </View>
  </ToggleBox>
</ScrollView>
```

## Props

|Prop name | Default prop | Required | Note
| --- | --- | --- | --- |
| `arrowColor` | `rgb(178, 178, 178)` | - | - |
| `arrowSize` | `30` | - | - |
| `arrowDownType` | `'keyboard-arrow-down'` | - | Icon name from`react-native-vector-icons/MaterialIcons` |
| `arrowUpType` | `'keyboard-arrow-up'` | - | Icon name from`react-native-vector-icons/MaterialIcons` |
| `children` | - | Yes | Element which you want to show inside of the box |
| `expanded` | `false` | - | Boolean if box should be expanded or not |
| `label` | - | Yes | Left label on the left of title |
| `style` | `{}` | - | Custom styles |
| `value` | `null` | - | Value on the right title |
