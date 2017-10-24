# ViewPagerIndicatorView

page indicator for android viewpager 

## HOW TO USE

1. put ViewPagerIndicatorView.java in your project

2. place ViewPagerIndicatorview in xml

```java
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:background="@color/colorPrimary">

    <android.support.v4.view.ViewPager
        android:id="@+id/vp"
        android:layout_width="match_parent"
        android:layout_height="200dp"
        android:layout_alignParentTop="true"
        android:layout_alignParentLeft="true"
        />

    <com.trend21c.viewpagerinrecyclerview.ViewPagerIndicatorView
        android:id="@+id/indicator"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_centerHorizontal="true"
        android:layout_alignParentBottom="true"
        android:layout_marginBottom="10dp"
        />

</RelativeLayout>
```

3. Init indicatorview

```java
ViewPagerIndicatorView indicatorView = (ViewPagerIndicatorView) findViewById(R.id.indicator);

int marginRight = 15;
int totalItemCount = getItemCount();
indicatorView.init(totalItemCount, R.drawable.dot, R.drawable.dot_on, marginRight);
indicatorView.setSelection(3);
```
