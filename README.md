# React native full screen functionality Android

There is plenty of room for improvment by adding additional react bindings for props and callbacks.

##### Usage:

```
    import FullScreen from 'react-native-full-screen';

    FullScreen.onFullScreen();

    FullScreen.onFullScreen();
```

##### Props: ToggleView

```html
  <ToggleView style={{flex:1,alignItems:'center', justifyContent:'center'}}>
    <Image style={{height:500,width:500}} source={{uri:"http://placehold.it/500"}}></Image>

  </ToggleView>
```

| Property | Type | Default | Description |
|---------------|----------|--------------|----------------------------------------------------------------|
| delay | number | 3000 | how long to delay hide |
| delayHide | boolean | true | if there should be a delayed hide event |


------------

## Android Installation

Install the npm package [`react-native-full-screen`](https://www.npmjs.com/package/react-native-full-screen). Inside your React Native project, run ([example](https://github.com/Anthonyzou/react-native-full-screen/tree/master/example)):
```bash
npm install --save react-native-full-screen
```

```
# RN >= 0.60
No action needed

# RN < 0.60
react-native link react-native-full-screen
```
### Manual installation


In `android/settings.gradle`, remove the line `include ':app'` and add the following lines
```
include ':react-native-full-screen'
project(':react-native-full-screen').projectDir = file('../node_modules/react-native-full-screen/android')
```
**NOTE** : If you have included other libraries in your project, the `include` line will contain the other dependencies too.

In `android/app/build.gradle`, add a dependency to `':react-native-full-screen'`

```
dependencies {
    compile project(':react-native-full-screen')
}
```

Next, you need to change the `MainActivity` of your app to register `FullScreenModule` :
```java
import com.rn.full.screen.FullScreenModule; // add this import

public class MainActivity extends ReactActivity {
    //...

    @Override
    protected List<ReactPackage> getPackages() {
      return Arrays.<ReactPackage>asList(
          new MainReactPackage(),
          new FullScreenModule() // add this manager
      );
    }
```

---

TeamLockr full screen
Team Lockr full screen for react native

These are functions created by the TeamLockr Team created for the TeamLockr platform.

---
