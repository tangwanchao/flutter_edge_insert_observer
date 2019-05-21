# edge_insert_observer

检测 Android,IOS EdgeInserts 完成事件,常用于键盘事件.

## 示例

```dart
class LoginPage extends StatefulWidget {
  @override
  _LoginPageState createState() => _LoginPageState();
}

class _LoginPageState extends State<LoginPage>
    with WidgetsBindingObserver, BottomInsertObserver {
    @override
    void bottomInsertComplete() {
        final double bottomInsert = MediaQuery.of(context).viewInsets.bottom;
        print(bottomInsert);
    }
}
```


