# sdk_release_android
-------

## Install SDK
Add the repositories url to your project-level `build.gradle`:
	
	repositories {
        maven { url "https://raw.githubusercontent.com/HyphenateInc/Hyphenate-SDK-Android/master/repository" }
    }

Add the following code to your module-level `build.gradle`:

	android {
   		//use legacy for android 6.0
    	useLibrary 'org.apache.http.legacy'
	}
	dependencies {
    	compile fileTree(dir: 'libs', include: '*.jar')
   		compile 'com.google.android.gms:play-services-gcm:9.4.0'
    	compile 'com.hyphenate:hyphenate-sdk:3.2.1'
	}

If you want use the sdk without voice/video calling, use `compile 'com.hyphenate:hyphenate-sdk-lite:3.2.1'`.

## Demo source code
Demo github link: [https://github.com/HyphenateInc/IMDemo_android](https://github.com/HyphenateInc/IMDemo_android "IMDemo")

Demo is dependent on EaseUI library project, EaseUI github link:[https://github.com/HyphenateInc/easeui_android](https://github.com/HyphenateInc/easeui_android "EaseUI")

**Remeber put the two projects in the same directory**
