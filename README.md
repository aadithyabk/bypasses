# bypasses
Repackaging of Bypass to allow for direct gradle dependencies

[![Build Status](https://travis-ci.org/Commit451/bypasses.svg?branch=master)](https://travis-ci.org/Commit451/bypasses)

# Gradle Dependency
Easily reference the library in your Android projects using this dependency in your module's `build.gradle` file:

# Gradle Dependency

Add this in your root `build.gradle` file (**not** your module `build.gradle` file):

```gradle
allprojects {
	repositories {
		...
		maven { url "https://jitpack.io" }
	}
}
```

Then, add the library to your project `build.gradle`
```gradle
dependencies {
    compile 'com.github.Commit451:bypasses:1.0.4'
}
```

This library is provided as a "fat" aar with native binaries for all available architectures. To
reduce your APK size, use the ABI filtering/splitting techniques in the Android plugin:
http://tools.android.com/tech-docs/new-build-system/user-guide/apk-splits

# Usage
See http://uncodin.github.io/bypass/

# Robolectric
See [this issue](https://github.com/Commit451/bypasses/issues/2) for an explination for getting Robolectric to work.

# Proguard
This dependency also packages the Proguard rules [suggested](https://github.com/Uncodin/bypass/issues/195) for bypass to work properly with Proguard enabled

License
--------

    Copyright 2015 Commit 451
    Copyright 2015 Uncodin

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

