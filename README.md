# xwjr_keyboard
# How To Use?
### 导包
    compile 'com.github.zhuxiaohang2016:xwjr_keyboard:1.1'
### 数据处理
###### xml
```` 
    <android.inputmethodservice.KeyboardView
        android:id="@+id/keyboardViewId"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:background="#D6D9DE"
        android:focusable="true"
        android:focusableInTouchMode="true"
        app:layout_constraintBottom_toBottomOf="parent"
        android:keyBackground="@drawable/keyboard_preview_layout"
        android:keyPreviewHeight="50dp"
        android:keyPreviewLayout="@layout/keyboard_key_btn"
        android:keyPreviewOffset="-5dp"
        android:keyTextColor="#747474"
        android:keyTextSize="12sp"
        android:paddingTop="10dp"
        android:paddingBottom="10dp"
        android:shadowRadius="0.0"
        android:visibility="gone" />
````
###### java
    new KeyboardUtil(a,b,c,d).showKeyboard(); //a:activity b:context c:edittext d:keyboardViewId
    //for example
    new KeyboardUtil(MainActivity.this, MainActivity.this, editText, R.id.keyboardView).showKeyboard();

### 注意事项
键盘样式已固定，如需变更，自行看xml文件修改
