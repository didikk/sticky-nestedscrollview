# StickyNestedScrollView
Upgraded version from [StickyScrollView](https://github.com/emilsjolander/StickyScrollViewItems)

## Installing
Add the following gradle dependency
```gradle
repositories {
    maven { url "https://jitpack.io" }
}

dependencies {
    compile 'com.github.didikk:sticky-nestedscrollview:1.0.0'
}
```

## Usage
Add android:tag="sticky" to your desired view.
```xml
<me.didik.component.StickyNestedScrollView
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@android:color/white"
    app:layout_behavior="@string/appbar_scrolling_view_behavior"
    tools:context="me.didik.stickynestedscrollview.MainActivity"
    tools:showIn="@layout/activity_main">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:padding="@dimen/activity_horizontal_margin">

        <TextView
            android:id="@+id/tv_title"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:background="@android:color/white"
            android:paddingBottom="10dp"
            android:paddingTop="10dp"
            android:tag="sticky"
            android:text="@string/sample"
            android:textColor="@color/colorAccent"
            android:textSize="18sp"/>

        // Other view

    </LinearLayout>

</me.didik.component.StickyNestedScrollView>
```