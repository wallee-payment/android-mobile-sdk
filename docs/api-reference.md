## API reference

| API | Type | Description |
| --- | :-: | --- |
| `WalleePaymentSdk.init(listener: OnResultEventListener)` | constructor | Initialization of SDK. Both Parameters are required! |
| `OnResultEventListener` | interface | Interface for handling post-payment events `paymentResult` |
| `fun paymentResult(paymentResult: PaymentResult)` | function | Result handler for transaction state |
| `WalleePaymentSdk.instance?.launch(token: String)` | function | Opening payment dialog (activity) |
| `WalleePaymentSdk.instance?.setDarkTheme(theme: JSONObject)` | function | Can override the whole dark theme or just some specific color. All colors are in json format |
| `WalleePaymentSdk.instance?.setLightTheme(theme: JSONObject)` | function | Can override the whole light theme or just some specific color. All colors are in json format |
| `WalleePaymentSdk.instance?.setCustomTheme(theme: JSONObject?, baseTheme: ThemeEnum)` | function | Force to use only this theme (independent on user's setup). Can override default light/dark theme and force to use it or completely replace all or specific colors |
| `WalleePaymentSdk.instance?.setAnimation(type: AnimationEnum)` | function | Defining type of animation for moving between the pages |
