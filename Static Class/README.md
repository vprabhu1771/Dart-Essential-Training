# The Dart Way: Mimicking a Static Class
To build a class that cannot be instantiated, extended, or implemented, and contains only static utilities, combine a private constructor with `abstract class` or the modern `abstract interface class` modifiers:
```dart
// A strict "Static" utility class simulation
abstract class CryptoUtils {
  // 1. Prevent instantiation by making the constructor private
  CryptoUtils._();

  // 2. Define static members
  static const String algorithm = 'AES-256';

  static String hashPassword(String password) {
    return 'hashed_$password'; // Example implementation
  }
}

void main() {
  // Usage: Access directly via the class name
  print(CryptoUtils.algorithm); 
  print(CryptoUtils.hashPassword('secret123'));

  // var utils = CryptoUtils(); // ERROR: Abstract classes cannot be instantiated
}
```
