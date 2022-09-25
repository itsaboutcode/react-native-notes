# React Native Notes

- `react` is a library that helps you create user interfaces.

- `react` is a platform-independent library.

- `react-dom` is the library on top of `react`, which helps you make web interfaces.

- `react-native` is the library on top of `react`, which helps you make mobile device interfaces.


## React Native

- `react-native` library provides you [UI components](https://reactnative.dev/docs/components-and-apis) library. Which are later compiled into native platforms.

- It also exposes platform-specific API to use the hardware of the device e.g., camera etc. 

- You should have knowledge `react` before you work on `react-native` but not required. You can learn the [core concepts](https://reactnative.dev/docs/intro-react) of `react` while learning `react-native` too.

- UI components/views are compiled to native views but JS logic is not compiled. It run in JS thread hosted by `react-native`

- `reacti-native` spins a JS process as part of your app and facilitates the communication between your JS code and compiled native components (also called a bridge).

## [Setting Up The Development Environment](https://reactnative.dev/docs/environment-setup)

You have 2 methods to setup your development environment.

1. Expo Go CLI (Third Party)
2. React Native CLI (Provided by `react` team)

Working with Expo Go CLI is easy as compare to work with React Native.

### Creating React Native Project

```
npx create-expo-app ProjectName
cd ProjectName
npm start
```

## Styling in React Native

## Layout with Flexbox

- `Flexbox` is all about organizing the child elements in **one dimentional** space.

- In `react-native`, every view `align` and `position` its **child views** using `flexbox`.

- By default, they are `aligned` in **column**.

- You can change the direction of `direction` of the views alignment using `flexDirection` property.

```
flexDirection: 'row|column|row-reverse|column-reverse'
```

## Flex Axis

- `main axis` : It is the direction of your flexbox.

- `cross axis`: It is the axis `perpendicular` to the main axis.


## Flex

- It defines how your items will **fill** the available space along your **main axis**.

- By default, if you don't spacify any flex property, it will only fill the space it needed for the content of child element on `main axis`.

- And by default, it will fill the maximum space available on the `cross axis`



<img width="679" alt="Screenshot 2022-09-25 at 1 29 49 PM" src="https://user-images.githubusercontent.com/204423/192134852-9e581f7e-2b55-48f7-9405-b885a7921e95.png">

# Libraries


# Reference Website

- https://reactjs.org/

- https://reactnative.dev/
