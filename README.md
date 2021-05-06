# TabLayoutChipStyleV1

- app
  - fr
    - [FirstFragment.java](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/java/com/gzeinnumer/tablayoutchipstylev1/fr/FirstFragment.java)
    - [SecondFragment.java](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/java/com/gzeinnumer/tablayoutchipstylev1/fr/SecondFragment.java)
  - [MainActivity.java](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/java/com/gzeinnumer/tablayoutchipstylev1/MainActivity.java)
  - [Utils.java](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/java/com/gzeinnumer/tablayoutchipstylev1/Utils.java)
  - [ViewPagerAdapter.java](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/java/com/gzeinnumer/tablayoutchipstylev1/ViewPagerAdapter.java)
- res
  - [chip_outline.xml](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/res/drawable/chip_outline.xml)
  - [chip_outline_selected.xml](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/res/drawable/chip_outline_selected.xml)
  - [selector_tab.xml](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/res/drawable/selector_tab.xml)
- layout
  - [activity_main.xml](https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/app/src/main/res/layout/activity_main.xml)

#

- activity_main.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@drawable/bg"
    android:orientation="vertical"
    tools:context=".MainActivity">

    <com.google.android.material.tabs.TabLayout
        android:id="@+id/tab_layout"
        android:layout_width="match_parent"
        android:layout_height="30dp"
        android:layout_gravity="center"
        android:background="@android:color/transparent"
        android:minWidth="80dp"
        android:minHeight="?attr/actionBarSize"
        app:tabBackground="@drawable/selector_tab"
        app:tabGravity="fill"
        app:tabIndicator="@drawable/chip_outline_selected"
        app:tabIndicatorColor="@android:color/transparent"
        app:tabIndicatorGravity="center"
        app:tabIndicatorHeight="30dp"
        app:tabMode="scrollable"
        app:tabRippleColor="@null"
        app:tabSelectedTextColor="@color/black"
        app:tabTextColor="@color/white" />

    <androidx.viewpager.widget.ViewPager
        android:id="@+id/view_pager"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        app:layout_behavior="@string/appbar_scrolling_view_behavior" />

</LinearLayout>
```

#

<p align="center">
  <img src="https://github.com/gzeinnumer/TabLayoutChipStyleV1/blob/master/preview/example1.jpg" width="400"/>
</p>

---

```
Copyright 2021 M. Fadli Zein
```