# 💬 Wegap Widget for Flutter / ویجت ویگپ برای Flutter

This repository contains the official Flutter version of the Wegap widget.  
این مخزن شامل نسخه رسمی ویجت ویگپ برای اپلیکیشن‌های Flutter است. با استفاده از این ویجت می‌توانید قابلیت‌هایی مانند **چت، تماس صوتی/تصویری و دانشیار هوش مصنوعی** را به راحتی به اپ خود اضافه کنید.

---

## 📦 Installation / نصب

در فایل `pubspec.yaml`:

```yaml
dependencies:
  wegap_widget_flutter: ^1.0.0
```

سپس:

```bash
flutter pub get
```

---

## 🚀 Quick Usage / استفاده سریع

```dart
import 'package:flutter/material.dart';
import 'package:wegap_widget_flutter/wegap_widget_flutter.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(title: const Text('Wegap Demo')),
        body: const Center(
          child: WegapWidget(
            authKey: 'YOUR_AUTH_KEY',
            theme: 'light',
            position: 'bottomRight',
            language: 'fa',
          ),
        ),
      ),
    );
  }
}
```

---

## ⚙️ Config Options / تنظیمات

| Prop Name | Type   | Description EN                                      | توضیح فارسی |
|-----------|--------|------------------------------------------------------|--------------|
| authKey   | string | Your unique authentication key                      | کلید احراز هویت شما |
| theme     | string | Theme mode: `light` or `dark`                       | تم: روشن یا تیره |
| position  | string | Widget position: `bottomRight`, `bottomLeft`, etc  | موقعیت ویجت |
| language  | string | Default widget language (fa, en, ar, ...)           | زبان پیش‌فرض |

---

## 📄 Documentation / مستندات کامل

- [See full guide in Wegap Wiki](https://wegap.net/wiki/flutter/نصب-و-راه-اندازی/راهنمای-ویجت-ویگپ/دانشیار-ویگپ-id-8915)
- مشاهده راهنما در ویکی ویگپ ↑
