```kotlin
@Composable
fun Icon(
    imageVector: ImageVector,
    contentDescription: String?,
    modifier: Modifier = Modifier,
    tint: Color = LocalContentColor.current.copy(alpha = LocalContentAlpha.current)
)
```


一个图标组件，使用 `tint` 可以修改 `Icon` 的颜色，默认为 `LocalContentColor`。对于一个可点击的图标，请查阅 [IconButton](iconbutton.md)。

``` kotlin
Row{
    Icon(Icons.Filled.ArrowBack, contentDescription = null)
    Icon(Icons.Filled.ArrowBack, contentDescription = null, tint = Color.Gray)
    Icon(Icons.Filled.ArrowBack, contentDescription = null, tint = Color.Red)
    Icon(Icons.Filled.ArrowBack, contentDescription = null, tint = Color.DarkGray)
    Icon(Icons.Filled.ArrowBack, contentDescription = null, tint = Color.Magenta)
    Icon(Icons.Filled.ArrowBack, contentDescription = null, tint = Color.Yellow)
    Icon(Icons.Filled.ArrowBack, contentDescription = null, tint = Color.Cyan)
}
```


![]({{config.assets}}/elements/icon/demo.png)