Fabric
======
This repository contains a CocoaPod for Fabric (https://fabric.io) for OS X.

### Current versions:
* Fabric.framework v1.2.4
* Crashlytics.framework v3.0.8

## Installing
1. Use Fabric Mac app to configure the components you need (required for this pod to work).
2. Remove all frameworks from project which were added by Fabric app.
3. Add pods to Podfile

```ruby
pod 'Fabric', '~> 1.2.4' # required
pod 'Fabric/Crashlytics', '~> 1.2.4'
```

  Then run `pod install`.

4. Change the path in Run Script Build command to:

  `./Pods/FabricOSX/Fabric.framework/run YOUR_API_KEY YOUR_BUILD_SECRET`
