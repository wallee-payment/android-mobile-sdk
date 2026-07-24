## Troubleshooting

Issue:

```gradle
Android resource linking failed
error: resource style/Theme.Design.Light.BottomSheetDialog (aka com.test.app.awesome:style/Theme.Design.Light.BottomSheetDialog) not found.
error: failed linking references.
```

Solution:

```gradle
implementation ("com.google.android.material:material:1.4.0")
```
