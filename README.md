# react-native-umeng-analytics-nevo

React Native Module for umeng analytics

## install

```
yarn add react-native-umeng-analytics-nevo
```

## Android

* init module (in Application.java)

```java
...

import com.umengs.analytics.RNUMConfigure;

public class MainApplication extends Application {

    ...

    @Override
    public void onCreate() {
        ...
        RNUMConfigure.init(this, "xxxx", "Umeng", UMConfigure.DEVICE_TYPE_PHONE, "");
    }
}
```

## iOS

### With Pod
```
pod install
```

* init module (in AppDelegate.m)

```objc
...

#import "RNUMConfigure.h"

- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
    ...
    [RNUMConfigure initWithAppkey:@"xxxxx" channel:@"AppleStore"];
}
```


### General Usage

```javascript
import Analytics from 'react-native-umeng-analytics-nevo';

```

```javascript
Analytics.onPageEnd('LoginScreen');

```
