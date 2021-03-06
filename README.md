# android-sdk-sample
Samples & documentation for the Straas Android SDK.

Developer Authentication
-----
Read [Credential](https://github.com/Straas/Straas-android-sdk-sample/wiki/SDK-Credential) first.

To run our sample, you have to copy your [`client_id`](https://github.com/Straas/Straas-android-sdk-sample/wiki/SDK-Credential#get-client-id) into [`gradle.properties`](https://github.com/Straas/Straas-android-sdk-sample/blob/master/gradle.properties#L8):
```
your_debug_client_id=xxxxx
your_release_client_id=xxxxx
```

User Identity
-----
Read [Identity](https://github.com/Straas/Straas-android-sdk-sample/wiki/User-Identity) first.
To change the identity in out sample, change the Identity declared in `MemberIdentity.ME`.

Using Straas Android SDK
-----
#### 1. Add repositories ####

Add repositories in the `build.gradle` file in the root of your project:

```gradle
repositories {
    google()
    jcenter()
    maven { url "https://raw.githubusercontent.com/Straas/Straas-android-sdk-releases/main" }
}
```

#### 2. Add Straas module dependencies ####

Then, add the dependencies in the `build.gradle` file of your app module:

X.X.X is the your preferred version. For the version information, see
[CHANGELOG](https://github.com/Straas/Straas-android-sdk-sample/blob/master/CHANGELOG.md)

- Media browser & playback + Ad integration (`minSdkVersion` 16):
```gradle
compile 'io.straas.android.sdk:straas-extension-ima:X.X.X'
```

- Media browser & playback only (`minSdkVersion` 16):
```gradle
compile 'io.straas.android.sdk:straas-media-core:X.X.X'
```

- ChatRoom  (`minSdkVersion` 14):
```gradle
compile 'io.straas.android.sdk:straas-messaging:X.X.X'
```

- ChatRoom with UI (`minSdkVersion` 14):
```gradle
compile 'io.straas.android.sdk:straas-messaging-ui:X.X.X'
```

- Streaming (`minSdkVersion` 18):
```gradle
compile 'io.straas.android.sdk:straas-streaming:X.X.X'
```

Learn about Android SDK
------------------
- [SDK Explained](https://github.com/Straas/android-sdk-sample/wiki)
