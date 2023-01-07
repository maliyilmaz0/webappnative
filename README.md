# webappnative

Hello everyone,

First of all you need to run 'npm install' command on your terminal.
Then you need to setup your Virtual Device like 'Android Studio or XCode'. 
All the instructions that you can find in https://reactnative.dev/docs/environment-setup

But then you need to solve a problem with react-native-camera package because it's not updated some of the hooks are removed from React.
All you need to find ./node_modules/react-native-camera/src/RNCamera.js and delete the 'ViewPropTypes' from import. 
Then add a new line 'import { ViewPropTypes } from 'deprecated-react-native-prop-types';' 

And then finally you can run project on your virtual device or your phone.

In the navigation folder you can find MainContainer.tsx that is responsible for bottom navigator and navigation.
In screens folder you can find HomeScreen.tsx is responsible for sending a http request on main server for start the python script i know it's not completed.
AddUser.tsx is responsible for taking photo and encoding it to base64 and posting it with new user's name and count of the photo with fetch.

The project is not completed. But If you have any question or issue with running project you can contact me.
