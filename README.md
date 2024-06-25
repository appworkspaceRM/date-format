# flutter_application_13

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

# Date Format

Date format merupakan pembentukan format dari sebuah tanggal, date format lebih udah menggunakan package intl dari package flutter dev yang bisa di tambahkan pada pubspec.yaml pada dependencies dari aplikasi yang akan di buat dengan mengimport

```bash
 flutter pub add intl
```

```dart
 import 'package:intl/intl.dart';
```

untuk date format menggunakan intl dengan melihat dan membaca dokumentasi dari package intl pada link


[intl - Dart API docs](https://pub.dev/documentation/intl/latest/)

```dart
import 'package:flutter/material.dart';
import 'package:intl/intl.dart';

void main(List<String> args) {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text(
            'Date Formatter',
          ),
        ),
        body: Center(
          child: Text(
            "${DateFormat.yMMMMEEEEd().add_jm().format(DateTime.now())}",
            style: const TextStyle(
              fontSize: 25,
            ),
          ),
        ),
      ),
    );
  }
}
```
![code-snapshot](https://github.com/appworkspaceRM/date-format/assets/135511281/d8e44549-9ffa-4d38-933c-1e387df4cbb9)
