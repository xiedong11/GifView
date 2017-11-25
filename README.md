# GifView [![](https://jitpack.io/v/xiedong11/GifView.svg)](https://jitpack.io/#xiedong11/GifView)

自定义View实现Gif图片加载

![Sample Screenshot](https://github.com/xiedong11/GifView/blob/master/picture/GIF.gif)

## Gradle

``` groovy
项目中添加jitpack仓库

allprojects {
		repositories {
			maven { url 'https://jitpack.io' }
		}
	}

在Module中添加依赖


dependencies {
     compile 'com.github.xiedong11:GifView:1.0'
    	}


如果你的项目中引入后，项目目依赖包发生Manifest Merge冲突，请在Module把依赖改成如下：
compile ('com.github.xiedong11:GifView:1.0'){
    exclude group: 'com.android.support'
}
```

## Usage

**XML**

``` xml
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.zhuandian.gif.MainActivity">

    <com.zhuandian.gifview.GifView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:gif="@mipmap/leaf" />

</android.support.constraint.ConstraintLayout>
```

**属性说明**

 * `gif` 被加载的Gif资源文件
