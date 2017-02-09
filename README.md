


AnimeWallpaper
=====================

Download high quality pictures from Konachan.net.


![Blur](blur.gif)

![Search](search.gif)


AppStore
--------
[Wandoujia](http://www.wandoujia.com/apps/com.github.miao1007.animewallpaper)




Build Environment
-------------
Android Studio 2.0 or higher


Feature
-------

####1. FullHD Wallpaper

1. download, preview and share full HD anime wallpaper for free.
2. search by name (eg. yosuga_no_sora)

####2. iOS design implementation for Android

1. Toolbar with translucent statusbar for Kitkat device above
2. Realtime blur on Android(Dialog/ActionSheet/ListView)
3. Search/Indicator(Progressbar)/Translation animation

####3. A practice with latest library

1. OkHttp/Picasso/Retrofit
2. RxJava


####4. Recommend iOS UIView for Android

see [iOS UIView for Android](github_best_ios.md)




Getting started
--------

#### 1. clone the project

  ```
git clone https://github.com/miao1007/AnimeWallpaper.git
  ```



#### 2. remove the SDK keys

this is my crash report's key, you can delete the config

first remove `buildConfigField` line in [build.gradle](https://github.com/miao1007/AnimeWallpaper/blob/master/app/build.gradle)

```diff
defaultConfig {
    applicationId "com.github.miao1007.animewallpaper"
    minSdkVersion 15
    targetSdkVersion 22
    versionCode 130
    versionName "1.3.0"
-   buildConfigField("String", "BUG_HD_SDK_GENERAL_KEY", BUG_HD_SDK_GENERAL_KEY)
  }
```

and remove following lines in [GlobalContext.java](https://github.com/miao1007/AnimeWallpaper/blob/master/app/src/main/java/com/github/miao1007/animewallpaper/support/GlobalContext.java)

```diff
public class GlobalContext extends Application {

-  FIR.init(instance,BuildConfig.BUG_HD_SDK_GENERAL_KEY);
-  FIR.addCustomizeValue("DEBUG", BuildConfig.DEBUG + "");
}
```

### 3. build the project

just click run




License
---------
1. Icon: [Creative Commons Attribution-NoDerivs 3.0 Unported](https://icons8.com/license/)
2. Font: [SIL OPEN FONT LICENSE Version 1.1 - 26 February 2007](https://www.google.com/fonts)



Developed By
-------------
Leon - miao1007@gmail.com

