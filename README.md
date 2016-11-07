# DateTimeShow
这是一个日期跟时间的显示控件
显示的格式yyyy-mm-dd-hh-mm
![image](https://github.com/m15115021148/DateTimeShow/blob/master/img/img1.jpeg)

布局如下：
  
  
    <?xml version="1.0" encoding="utf-8"?>
    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:orientation="vertical"
    android:gravity="center_vertical"
    android:background="@drawable/layout_bg">


    <TextView
        android:textColor="#007AFF"
        android:textSize="@dimen/_40px_in720p"
        android:gravity="left"
        android:padding="@dimen/_30px_in720p"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="请选择日期与时间" />
    <View
        android:background="#007AFF"
        android:layout_width="match_parent"
        android:layout_height="@dimen/_2px_in720p"/>

    <LinearLayout
        android:layout_marginTop="@dimen/_10px_in720p"
        android:id="@+id/timePicker1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:padding="@dimen/_20px_in720p">

        <com.sitemap.datetimeshow.view.WheelTimeView
            android:id="@+id/year"
            android:layout_width="@dimen/_150px_in720p"
            android:layout_height="wrap_content" />

        <com.sitemap.datetimeshow.view.WheelTimeView
            android:id="@+id/month"
            android:layout_width="@dimen/_100px_in720p"
            android:layout_height="wrap_content" />

        <com.sitemap.datetimeshow.view.WheelTimeView
            android:id="@+id/day"
            android:layout_width="@dimen/_100px_in720p"
            android:layout_height="wrap_content" />

        <com.sitemap.datetimeshow.view.WheelTimeView
            android:id="@+id/hour"
            android:layout_width="@dimen/_100px_in720p"
            android:layout_height="wrap_content" />

        <com.sitemap.datetimeshow.view.WheelTimeView
            android:id="@+id/mins"
            android:layout_width="@dimen/_100px_in720p"
            android:layout_height="wrap_content" />
    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="@dimen/_20px_in720p">

        <Button
            android:id="@+id/btn_datetime_cancel"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="取消"></Button>

        <Button
            android:id="@+id/btn_datetime_sure"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="确定"></Button>


    </LinearLayout>

    </LinearLayout>
