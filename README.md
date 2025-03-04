# React Native Notes

- `react` is a library that helps you create user interfaces.

- `react` is a platform-independent library.

- `react-dom` is the library on top of `react`, which helps you make web interfaces.

- `react-native` is the library on top of `react`, which helps you make mobile device interfaces.


## React Native

- `react-native` library provides you [UI components](https://reactnative.dev/docs/components-and-apis) library. Which are later compiled into native platforms.

- It also exposes platform-specific API to use the hardware of the device, e.g., camera, etc. 

- You should know about `react` before you work on `react-native,` but it is not required. You can learn the [core concepts](https://reactnative.dev/docs/intro-react) of `react` while learning `react-native` too.

- UI components/views are compiled to native views, but JS logic is not compiled. It runs in JS thread hosted by `react-native`

- `reacti-native` spins a JS process as part of your app and facilitates the communication between your JS code and compiled native components (also called a bridge).

## [Setting Up The Development Environment](https://reactnative.dev/docs/environment-setup)

You have 2 methods to set up your development environment.

1. Expo Go CLI (Third Party)
2. React Native CLI (Provided by `react` team)

Working with Expo Go CLI is easy compared to working with React Native.

### Creating the Expo CLI Project and Running It

```
npx create-expo-app@latest ProjectName
cd ProjectName
npm start                           # Running it
```

### Creating Native CLI Project

- Make sure `react-native-cli` is not installed. If installed, uninstall it using the following command.

```
npm uninstall -g react-native-cli @react-native-community/cli
```

Now, create a project

```
npx react-native@latest init AwesomeProject
```

### Running your Native CLI application

**Step 1:** Start Metro

- It's a JavaScript **bundler**.

- It "takes in an entry file and various options, and returns a single JavaScript file that includes all your code and its dependencies."

```
npx react-native start
```

**Step 2:** Start your application 

- Android command

```
npx react-native run-android
```

You can do step 2, and it will automatically execute step 1.

To run the application on your physical device and enable the [developer mode](https://developer.android.com/studio/debug/dev-options) on your device and allow debugging.

## UI Controls

### View

- It's like `div` in HTML

## Styling in React Native

- All UI controls have a `style` prop, which you can use to to style UI controls.
- You create a `Stylesheet` object

```
const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#0000',
  },
});
```

- Assing it to your respective control

```
<View style={styles.container}></View>
```

## Debugging using the console and developer menu

- console.log # Make sure you remove this before releasing the app because it impacts the performance of your app.
- On an Android device, shake it, and it will show you the  developer menu
- Android Simulator, CTRL/CMD+M
- iOS Simulator, CTRL/CMD+D

## Layout with Flexbox

- `Flexbox` is all about organizing the child elements in **one dimensional** space.

- In `react-native`, every view `align` and `position` its **child views** using `flexbox`.

- By default, they are `aligned` in the **column**.

- You can change the direction of the `direction` of the views alignment using the `flexDirection` property.

```
flexDirection: 'row|column|row-reverse|column-reverse'
```

## Flex Axis

- `main axis`: It is the direction of your flexbox.

- `cross axis`: It is the axis `perpendicular` to the main axis.


## Flex

- It defines how your items will **fill** the available space along your **main axis**.

- By default, if you don't specify any flex property, it will only fill the space it needs for the content of cthe hild element on the `main axis`.

- And by default, it will fill the maximum space available on the `cross axis`



<img width="679" alt="Screenshot 2022-09-25 at 1 29 49 PM" src="https://user-images.githubusercontent.com/204423/192134852-9e581f7e-2b55-48f7-9405-b885a7921e95.png">

## Content Default Behaviour

- When `flexDirection` is `column`, `height` is `auto` for inner containers (height of the content) and `width` is 100%.


![flex-column](https://user-images.githubusercontent.com/204423/192433529-9e3cc423-3354-44f1-a0e3-9deb71b58f99.png)

- When `flexDirection` is `row`, `height` and `width` is `auto` for inner containers (height of the content).


![flex-row](https://user-images.githubusercontent.com/204423/192433559-b75db324-7034-49c3-a686-3085f25b9458.png)


## ReactJS Required Knowledge For React Native


# Libraries


# Reference Website

- https://reactjs.org/

- https://reactnative.dev/

- https://snack.expo.dev/

- https://expo.dev/

- https://www.nativewind.dev/

- https://redux.js.org/

- https://reactnavigation.org/

- https://www.sanity.io/
