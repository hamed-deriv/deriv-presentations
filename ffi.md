```



'||''''|  '||''''|  '||'
 ||  .     ||  .     ||
 ||''|     ||''|     ||
 ||        ||        ||
.||.      .||.      .||.





```

#### - FFI stands for foreign function interface.

#### - Binding to native code.

#### - Flutter can use the 'dart:ffi' library to call native C APIs.

---

## Statically linked library

    A statically linked library is embedded into the app’s executable image, and is loaded when the app starts.

## Dynamically linked library

    A dynamically linked library, is distributed in a separate file or folder within the app, and loaded on-demand.

---

## FFI library types

    - First-party library

    - Open-source third-party

    - Closed-source third-party library

---

## Create a plugin

```dart
$ flutter create --platforms=android,ios --template=plugin <PLUGIN NAME>
```

## Add C/C++ sources

```c
#include <stdint.h>

char* getSimpleString() {
    return "SIMPLE STRING";
}
```

## Add CMake

#### create a 'CMakeLists.txt' file to define how the sources should be compiled and point Gradle to it.

```bash
add_library(
    <CLASS NAME>
    SHARED
    ../ios/Classes/<CLASS NAME>.cpp
)
```

#### add an externalNativeBuild section to 'android/build.gradle'.

```json
android {
  externalNativeBuild {
    cmake {
      path "CMakeLists.txt"
    }
  }
}
```

---

## Using FFI

```dart
final DynamicLibrary _nativeAppTokenLib = Platform.isAndroid
    ? DynamicLibrary.open('libnative_app_token.so')
    : DynamicLibrary.process();

final Pointer<Utf8> Function() _getSimpleString = _nativeAppTokenLib
    .lookup<NativeFunction<Pointer<Utf8> Function()>>('getSimpleString')
    .asFunction();

String get getSimpleString => _getSimpleString().toDartString();
```

---

```










           _   _ __     __   ____   _    _  ______   _____  _______  _____  ____   _   _  ___
    /\    | \ | |\ \   / /  / __ \ | |  | ||  ____| / ____||__   __||_   _|/ __ \ | \ | | |__ \
   /  \   |  \| | \ \_/ /  | |  | || |  | || |__   | (___     | |     | | | |  | ||  \| |   ) |
  / /\ \  | . . |  \   /   | |  | || |  | ||  __|   \___ \    | |     | | | |  | || . . |  / /
 / ____ \ | |\  |   | |    | |__| || |__| || |____  ____) |   | |    _| |_| |__| || |\  | |_|
/_/    \_\|_| \_|   |_|     \___\_\ \____/ |______||_____/    |_|   |_____|\____/ |_| \_| (_)
```

## https://flutter.dev/docs/development/platform-integration/c-interop
