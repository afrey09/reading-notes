React Native

Getting started with react native:
1. Name three core components of React Native and describe what they do:
  - View: A container that supports layout with flexbox, style, some touch handling, and accessibility controls.. designed to be nested inside other views and to have 0 to many children of any type.
  - Text: A React component for displaying text which supports nesting, styling, and touch handling.
  - ScrollView: A generic scrolling container that can contain multiple components and views. ScrollView can be used horizontal and vertically.
  - Image: A React component for displaying different types of images, including network images, static resources, temporary local images, and images from local disk, such as the camera roll.
  - TextInput: A React component for entering text. This is a controlled component that requires an onChangeText callback that updates the value prop in order for the component to reflect user input.

  2. What problem does React Native solve(why call it native)? "React Native is an open source framework for building Android and iOS applications using React and the app platform’s native capabilities. With React Native, you use JavaScript to access your platform’s APIs as well as to describe the appearance and behavior of your UI using React components: bundles of reusable, nestable code." 

  3. What are the building blocks of a React Native app?  
    Text and View components are the building blocks of a React Native app. Text is used to display text on the screen and View is used to layout other components. 

    How does that compare to a React app? 

    source: https://reactnative.dev/docs/intro-react-native-components

  expo

  1. What solution does expo provide? "Expo is an open-source framework for apps that run natively on Android, iOS, and the web. Expo brings together the best of mobile and the web and enables many important features for building and scaling an app.

    The expo npm package enables a suite of incredible features for React Native apps. The expo package can be installed in nearly any React Native project."

  2. Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the __bare__ workflow

  3. What is the difference between React Native and Expo? "React Native is a framework for building native apps using React. Expo is a set of tools built around React Native for developing, building, and deploying apps."

source: https://docs.expo.dev/home/core-concepts/?redirected
        https://docs.expo.dev/workflow/customizing/

  expo snack

  1. What does snack allow you to do? Snack is an online code editor specifically for React Native. It allows you to write code and see the result of running that code such as with Replit or Codepen.

  source: https://snack.expo.dev/

  ejecting

  1. What does "eject" mean within the context of Expo? 
    "The term "eject" was popularized by create-react-app, and it is used in Expo to describe leaving the cozy comfort of the standard Expo development environment, where you do not have to deal with build configuration or native code. 

  2. When should you not eject? When the build configuration or native code is beneficial to your project.

  3. When might you choose to eject? When you need to customize the build configuration or native code.

source:https://docs.expo.dev/archive/glossary/#eject?redirected