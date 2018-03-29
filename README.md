# Lottie for Android, [Official website](https://github.com/airbnb/lottie-android),

just for fix a bug in lotti-android 2.2.0.

cherry-pick 
'''
commit 40eace73c1102477c4bb7b86a5e9843c230ebf11
Author: Gabriel Peal <gabriel.peal@airbnb.com>
Date:   Mon Dec 11 22:38:34 2017 -0500

    Use a different method for splitting the version string
    
    I think some devices have a broken regex function that causes
    split to fail on the current regex. This version may work better.
    Fixes #559

'''

## Download

Gradle is the only supported build configuration, so just add the dependency to your project `build.gradle` file:

```groovy
	allprojects {
		repositories {
			...
			maven { url 'https://www.jitpack.io' }
		}
	}
  
  dependencies {
      compile 'com.github.bborn2:lottie-android:v2.2.0_patch-SNAPSHOT'
  }
```
