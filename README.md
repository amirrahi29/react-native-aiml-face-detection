```

Face-Detection-React-Native

##setup env

Add the folowing to project level build.gradle:
==========================================================================================
buildscript {
  dependencies {
  // Add this line
  classpath 'com.google.android.gms:strict-version-matcher-plugin:1.2.1' // <--- you might want to use different version
  }
}

```
add to the bottom of android/app/build.gradle file
==========================================================================================
apply plugin: 'com.google.android.gms.strict-version-matcher-plugin'

```
android {
  defaultConfig {
  ...
  missingDimensionStrategy 'react-native-camera', 'mlkit'
