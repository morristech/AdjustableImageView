# AdjustableImageView

Provide `AdjustableImageView` and `AdjustableImageButton` to correct the **adjustViewBounds** behavior of ImageView and ImageButton when run on API Level 17 and below.

![](http://inthecheesefactory.com/uploads/source/adjustableimageview/final.png)

Related article about this library is written at http://inthecheesefactory.com/blog/correct-imageview-adjustviewbounds-with-adjustable-imageview/en

# Version

1.0.1

# Installation

To use this library in your android project, just simply add the following dependency into your build.gradle

```sh
dependencies {
    compile 'com.inthecheesefactory.thecheeselibrary:adjustable-imageview:1.0.1'
}
```

# Usage

Replace your ImageView with `com.inthecheesefactory.thecheeselibrary.widget.AdjustableImageView` and replace your ImageButton with `com.inthecheesefactory.thecheeselibrary.widget.AdjustableImageButton`, for example:

```xml
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context=".MainActivity">

    <ScrollView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:fillViewport="true">

        <LinearLayout android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:orientation="vertical">

            <com.inthecheesefactory.thecheeselibrary.widget.AdjustableImageView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:adjustViewBounds="true"
                android:src="@mipmap/ic_launcher"/>

            <com.inthecheesefactory.thecheeselibrary.widget.AdjustableImageView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:adjustViewBounds="true"
                android:src="@mipmap/ic_launcher"/>
        </LinearLayout>

    </ScrollView>

</LinearLayout>
```

# Change Logs

### v1.0.1

Fix some bug with manifest merger

### v1.0.0

Initial version

# License
Apache 2.0
