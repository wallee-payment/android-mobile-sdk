# Table of contents

- [Table of contents](#table-of-contents)
- [wallee Android Payment SDK](#wallee-android-payment-sdk)
  - [Installation](#installation)
- [Wallee Android SDK — Migration Guide v2.0.0](#wallee-android-sdk--migration-guide-v200)
  - [Requirements](#requirements)
  - [Installation](#installation-1)
  - [What's new](#whats-new)
  - [Documentation](#documentation)

# wallee Android Payment SDK

[![Maven Central](https://img.shields.io/maven-central/v/com.wallee/wallee-payment-sdk)](https://central.sonatype.com/artifact/com.wallee/wallee-payment-sdk/)

## Installation

# Wallee Android SDK — Migration Guide v2.0.0

## Requirements

|                             | Version |
| --------------------------- | ------- |
| Kotlin                      | 2.1.20  |
| Android Gradle Plugin (AGP) | 8.7.0   |

## Installation

Latest version: **2.0.0** — [Maven Central](https://central.sonatype.com/artifact/com.wallee/wallee-payment-sdk/)

Add the dependency to your `build.gradle.kts`:

```kotlin
implementation("com.wallee:wallee-payment-sdk:2.0.0")
```

---

## What's new

Version 2.0.0 brings a complete architectural overhaul of the SDK. The public API and component behavior remain unchanged — the only breaking change is the **entry class rename**.

The architecture has also been updated to comply with the **Android 16KB page size alignment requirement**, ensuring compatibility with devices running on 16KB memory page sizes as required by Google. For more details, see the [official Android documentation](https://developer.android.com/guide/practices/page-sizes).

> **Still seeing 16KB alignment issues in your app?**
> The problem may be caused by other libraries or an outdated build toolchain in your project. We recommend upgrading to **AGP 8.7.0 or higher** and updating your other dependencies to their latest versions.

---

## Documentation

- [API Reference](./docs/api-reference.md)
- [Integration](./docs/integration.md)
- [Theming](./docs/theming.md)
- [Troubleshooting](./docs/troubleshooting.md)
