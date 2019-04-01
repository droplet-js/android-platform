# android-platform

[![Build Status](https://cloud.drone.io/api/badges/v7lin/android-platform/status.svg)](https://cloud.drone.io/v7lin/android-platform)
[![GitHub tag](https://img.shields.io/github/tag/v7lin/android-platform.svg)](https://github.com/v7lin/android-platform/releases)
[![API](https://img.shields.io/badge/API-14%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=14)

### snapshot

````
ext {
    latestVersion = '0.0.2-SNAPSHOT'
}

allprojects {
    repositories {
        ...
        maven {
            url 'https://oss.jfrog.org/artifactory/oss-snapshot-local'
        }
        ...
    }
}
````

### release

````
ext {
    latestVersion = '0.0.2'
}

allprojects {
    repositories {
        ...
        jcenter()
        ...
    }
}
````

### usage

android
````
...
dependencies {
    ...
    implementation "io.github.v7lin:platform-compatibility-android:${latestVersion}"
    ...
}
...
````
