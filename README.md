# patched for offline workers bundle
------------------------------------
1. install as per [README-ORIG.md](README-ORIG.md)
2. copy ios/react-native-workers.sh to same location in your app
3. edit react-native-workers.sh with path to your workers
4. update xcode Build Phases -> Bundle React Native code and images with:
```
    export NODE_BINARY=node
    ./react-native-workers.sh
    ../node_modules/react-native/packager/react-native-xcode.sh
```

Profit!
