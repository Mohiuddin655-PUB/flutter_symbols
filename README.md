# flutter_symbols

## Use case
```dart

IconData icon = SymbolIcons.rightAngleWithZigzagArrow;
Symbol symbol = Symbols.rightAngleWithZigzagArrow;
```
## Example
```dart
import 'package:flutter/material.dart';
import 'package:flutter_symbols/flutter_symbols.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Symbols',
      theme: ThemeData(
        colorScheme: ColorScheme.fromSeed(seedColor: Colors.deepPurple),
        useMaterial3: true,
      ),
      home: Scaffold(
        body: Padding(
          padding: const EdgeInsets.all(50),
          child: Center(
            child: Column(
              mainAxisSize: MainAxisSize.min,
              children: [
                const Icon(
                  SymbolIcons.rightAngleWithZigzagArrow,
                  size: 50,
                  fill: 0.3,
                  color: Colors.red,
                ),
                const SizedBox(height: 32),
                Text(
                  "\"${Symbols.rightAngleWithZigzagArrow.symbol}\" this is a \"${Symbols.rightAngleWithZigzagArrow.id}\" symbol",
                  style: const TextStyle(
                    color: Colors.black,
                    fontSize: 32,
                  ),
                  textAlign: TextAlign.center,
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}
```