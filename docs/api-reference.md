## API reference

| API | Type | Description |
| --- | :-: | --- |
| `WalleePaymentSdk.init(listener: OnResultEventListener)` | function | Initializes the SDK and registers the result listener. Must be called before using `WalleePaymentSdk.instance`. |
| `WalleePaymentSdk.instance` | singleton | Shared SDK instance used for configuration and launching payments. |
| `OnResultEventListener` | interface | Interface for handling post-payment events (`paymentResult`). |
| `fun paymentResult(paymentResult: PaymentResult)` | function | Callback invoked when transaction state changes or payment is completed. |
| `WalleePaymentSdk.instance?.launch(token: String, context: Context)` | function | Opens the payment flow. |
| `WalleePaymentSdk.instance?.launch(token: String, context: Context, paymentMethodConfigurationId: Int? = null)` | function | Opens the payment flow. `paymentMethodConfigurationId` is optional and can be used to preselect a payment method. |
| `WalleePaymentSdk.instance?.setDarkTheme(theme: JSONObject)` | function | Overrides or extends the default dark theme colors. |
| `WalleePaymentSdk.instance?.setLightTheme(theme: JSONObject)` | function | Overrides or extends the default light theme colors. |
| `WalleePaymentSdk.instance?.setCustomTheme(theme: JSONObject?, baseTheme: ThemeEnum)` | function | Forces a custom theme regardless of system appearance. Missing values are merged with the selected base theme. |
| `WalleePaymentSdk.instance?.setAnimation(type: AnimationEnum)` | function | Sets transition animation style used inside the payment flow. |
| `WalleePaymentSdk.instance?.SDK_VERSION` | property | Current SDK version. |
