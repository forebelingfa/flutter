# 7-Day Flutter Zero-to-Hero Plan

## Day 1: Getting Started with Flutter
- **Install Flutter**: 
  - Follow the [official installation guide](https://flutter.dev/docs/get-started/install).
- **Set Up Your Environment**: 
  - Install an IDE (VS Code or Android Studio).
  - Set up the Flutter and Dart plugins in your IDE.
- **Create Your First App**:
  - Run `flutter create my_first_app`.
  - Explore the default app and run it on an emulator or device.

## Day 2: Dart Basics
- **Learn Dart**: 
  - Read through the [Dart language tour](https://dart.dev/tutorials/language).
- **Practice Basic Concepts**:
  - Variables, data types, functions, and control flow (if, for, while).
- **Hands-On Project**:
  - Create a simple Dart console application to practice.

## Day 3: Flutter Widgets
- **Understand Widgets**: 
  - Learn about Stateless and Stateful widgets.
- **Explore Common Widgets**:
  - Text, Container, Row, Column, ListView, and Stack.
- **Build a Simple UI**:
  - Create a layout using various widgets to display a list of items.

## Day 4: State Management
- **Learn About State Management**:
  - Understand the difference between local and global state.
- **Explore Provider**:
  - Follow a tutorial on using the Provider package for state management.
- **Implement a Simple State Management Example**:
  - Create a counter app using Provider to manage the state.

## Day 5: Navigation and Routing
- **Understand Navigation**:
  - Learn about navigating between screens (routes).
- **Implement Named Routes**:
  - Create a multi-screen app using named routes.
- **Add a Bottom Navigation Bar**:
  - Implement a bottom navigation bar to switch between different screens.

## Day 6: Networking and APIs
- **Learn About HTTP Requests**:
  - Use the `http` package to make network requests.
- **Consume a Public API**:
  - Fetch data from a public API (e.g., JSONPlaceholder) and display it in your app.
- **Error Handling**:
  - Implement error handling for network requests.

## Day 7: Build a Complete App
- **Choose a Simple App Idea**:
  - For example, a to-do list, weather app, or notes app.
- **Plan Your App**:
  - Outline features and UI components.
- **Develop the App**:
  - Implement all the concepts learned over the week.
- **Test and Debug**:
  - Test your app on different devices and fix any issues.
- **Deploy**:
  - Follow the steps to prepare your app for release (optional).

## Additional Tips:
- **Practice Daily**: Spend at least 2-3 hours each day coding.
- **Join the Community**: Engage with Flutter communities on platforms like Discord, Reddit, or Stack Overflow.
- **Refer to Documentation**: The [Flutter documentation](https://flutter.dev/docs) is comprehensive and a valuable resource.

By the end of this week, you should have a solid understanding of Flutter and a functional app to showcase your skills!

Here's an expanded version of Day 1 for your Flutter learning plan:

```markdown
## Day 1: Getting Started with Flutter

### 1. Install Flutter
- **Follow the Official Installation Guide**:
  - Visit the [Flutter installation guide](https://flutter.dev/docs/get-started/install).
  - Choose your operating system (Windows, macOS, or Linux) and follow the steps to download and install Flutter SDK.
  
### 2. Set Up Your Environment
- **Install an IDE**:
  - **Visual Studio Code**:
    - Download and install from [Visual Studio Code](https://code.visualstudio.com/).
    - Install the Dart and Flutter plugins:
      - Open VS Code.
      - Go to Extensions (`Ctrl+Shift+X`).
      - Search for "Flutter" and install it (this will also install the Dart plugin).
  
  - **Android Studio**:
    - Download and install from [Android Studio](https://developer.android.com/studio).
    - During installation, ensure that you install the Android SDK and set up the Android Emulator.
    - Open Android Studio, go to **Preferences** > **Plugins**, and search for "Flutter" to install it (this will also install the Dart plugin).

### 3. Verify Your Installation
- Open a terminal (Command Prompt, PowerShell, or Terminal) and run:
  ```bash
  flutter doctor
  ```
- This command checks your environment and displays a report of the status of your Flutter installation. Make sure there are no issues.

### 4. Create Your First App
- **Run the Command**:
  - In your terminal, navigate to your preferred project directory and run:
    ```bash
    flutter create my_first_app
    ```
- **Explore the Project Structure**:
  - Navigate into your project folder:
    ```bash
    cd my_first_app
    ```
  - Open the project in your IDE (VS Code or Android Studio).
  - Familiarize yourself with the following folders and files:
    - **lib/**: Contains the main Dart code for your app (main.dart is the entry point).
    - **pubspec.yaml**: Manages assets, dependencies, and metadata for your app.
    - **android/** & **ios/**: Platform-specific code for Android and iOS.

### 5. Run Your App
- **Start an Emulator or Connect a Device**:
  - For Android, open the AVD Manager in Android Studio and launch an emulator.
  - For iOS, use Xcode to start a simulator (macOS only).
  
- **Run the App**:
  - In your terminal, within the project directory, run:
    ```bash
    flutter run
    ```
  - Alternatively, use the run button in your IDE.

### 6. Explore the Default App
- **Review the UI**:
  - The default app displays "You have pushed the button this many times:" along with a counter.
  
- **Modify the App**:
  - Open `lib/main.dart` and try the following changes:
    - Change the title in the `appBar` to something like "My First Flutter App".
    - Modify the text in the body to display a welcome message.

### 7. Learn Basic Commands
- Familiarize yourself with these common Flutter commands:
  - `flutter pub get`: Fetches dependencies listed in `pubspec.yaml`.
  - `flutter run`: Runs the app on an emulator or connected device.
  - `flutter build`: Builds the app for release.
  - `flutter analyze`: Analyzes the project for potential issues.

### 8. Resources for Further Learning
- **Flutter Documentation**: [Flutter Docs](https://flutter.dev/docs)
- **Dart Language Tour**: [Dart Tour](https://dart.dev/tutorials/language)
- **Flutter YouTube Channel**: Explore video tutorials for visual learning.

By the end of Day 1, you should have Flutter installed, your first app created and running, and a basic understanding of the project structure.
```

This expanded version provides a more detailed guide for Day 1, covering installation, setup, and initial exploration of Flutter. Feel free to adjust any sections to better suit your learning style!
Here's an expanded version of Day 2 for your Flutter learning plan:

```markdown
## Day 2: Dart Basics

### 1. Introduction to Dart
- **What is Dart?**
  - Dart is the programming language used for building Flutter applications. It is object-oriented, strongly typed, and supports both just-in-time (JIT) and ahead-of-time (AOT) compilation.

### 2. Set Up Dart Environment
- **Dart SDK**:
  - When you install Flutter, the Dart SDK is included. You can check your Dart version by running:
    ```bash
    dart --version
    ```

### 3. Learn Dart Basics
- **Variables and Data Types**:
  - Understand the basic data types: `int`, `double`, `String`, `bool`, `List`, and `Map`.
  - Example:
    ```dart
    int age = 30;
    double height = 5.9;
    String name = "Alice";
    bool isStudent = false;
    List<String> fruits = ["Apple", "Banana", "Cherry"];
    Map<String, int> scores = {"Math": 90, "English": 85};
    ```

- **Control Flow**:
  - **Conditional Statements**:
    - Learn about `if`, `else if`, and `else` statements.
    ```dart
    if (age > 18) {
      print("Adult");
    } else {
      print("Minor");
    }
    ```

  - **Loops**:
    - Explore `for`, `while`, and `do-while` loops.
    ```dart
    for (var fruit in fruits) {
      print(fruit);
    }
    ```

### 4. Functions
- **Defining Functions**:
  - Learn how to define and call functions.
  ```dart
  void greet(String name) {
    print("Hello, $name!");
  }

  greet("Alice");
  ```

- **Returning Values**:
  - Functions can return values.
  ```dart
  int add(int a, int b) {
    return a + b;
  }

  var sum = add(5, 3);
  print(sum); // Outputs: 8
  ```

### 5. Collections
- **Lists**:
  - Learn how to create and manipulate lists.
  ```dart
  List<int> numbers = [1, 2, 3];
  numbers.add(4);
  print(numbers); // Outputs: [1, 2, 3, 4]
  ```

- **Maps**:
  - Understand how to use maps to store key-value pairs.
  ```dart
  Map<String, String> capitals = {
    "USA": "Washington, D.C.",
    "France": "Paris"
  };
  print(capitals["France"]); // Outputs: Paris
  ```

### 6. Practice Basic Concepts
- **Hands-On Project**:
  - Create a simple Dart console application to practice.
  - Example Project: A simple calculator that performs addition, subtraction, multiplication, and division.
  
```dart
import 'dart:io';

void main() {
  print("Enter first number:");
  double num1 = double.parse(stdin.readLineSync()!);

  print("Enter second number:");
  double num2 = double.parse(stdin.readLineSync()!);

  print("Select operation: +, -, *, /");
  String operation = stdin.readLineSync()!;

  double result;

  switch (operation) {
    case '+':
      result = num1 + num2;
      break;
    case '-':
      result = num1 - num2;
      break;
    case '*':
      result = num1 * num2;
      break;
    case '/':
      result = num1 / num2;
      break;
    default:
      print("Invalid operation");
      return;
  }

  print("Result: $result");
}
```

### 7. Additional Resources
- **Dart Documentation**: [Dart Official Documentation](https://dart.dev/guides)
- **Dart Language Tour**: [Dart Language Tour](https://dart.dev/tutorials/language)
- **DartPad**: [DartPad](https://dartpad.dev/) - An online editor to practice Dart code.

### 8. Summary
By the end of Day 2, you should have a solid understanding of Dart's basic syntax, data types, control flow, and functions. You'll also have hands-on experience creating a simple console application.
```

This expanded Day 2 plan provides a comprehensive overview of Dart basics, including practical examples and a mini-project to reinforce learning. Feel free to adapt any sections to better fit your style!
Here's an expanded version of Day 3 for your Flutter learning plan:

```markdown
## Day 3: Flutter Widgets

### 1. Understanding Widgets
- **What are Widgets?**
  - Widgets are the building blocks of a Flutter app's user interface. Every element in a Flutter app, from buttons to layouts, is a widget.
  
- **Types of Widgets**:
  - **Stateless Widgets**: Immutable widgets that don’t change their state. They are useful for static content.
  - **Stateful Widgets**: Widgets that maintain state and can change dynamically. They are used for interactive content.

### 2. Setting Up a Basic App
- **Create a New Flutter App**:
  - If you haven't already, create a new Flutter project:
    ```bash
    flutter create my_widget_app
    cd my_widget_app
    ```
  
- **Open the Project** in your IDE.

### 3. Exploring Common Widgets
- **Text Widget**:
  - Displays a string of text with single style.
  ```dart
  Text('Hello, Flutter!', style: TextStyle(fontSize: 24));
  ```

- **Container Widget**:
  - A box model that can contain other widgets and apply padding, margin, and decoration.
  ```dart
  Container(
    padding: EdgeInsets.all(16.0),
    margin: EdgeInsets.symmetric(vertical: 10.0),
    color: Colors.blue,
    child: Text('This is a Container'),
  );
  ```

- **Row and Column Widgets**:
  - Used for horizontal and vertical layouts, respectively.
  ```dart
  Row(
    mainAxisAlignment: MainAxisAlignment.spaceAround,
    children: [
      Icon(Icons.star),
      Icon(Icons.star),
      Icon(Icons.star),
    ],
  );

  Column(
    mainAxisAlignment: MainAxisAlignment.center,
    children: [
      Text('Item 1'),
      Text('Item 2'),
      Text('Item 3'),
    ],
  );
  ```

- **ListView Widget**:
  - A scrollable list of widgets.
  ```dart
  ListView(
    children: [
      ListTile(title: Text('Item 1')),
      ListTile(title: Text('Item 2')),
      ListTile(title: Text('Item 3')),
    ],
  );
  ```

- **Stack Widget**:
  - Allows you to stack widgets on top of each other.
  ```dart
  Stack(
    children: [
      Container(color: Colors.blue, width: 100, height: 100),
      Positioned(
        left: 20,
        top: 20,
        child: Container(color: Colors.red, width: 60, height: 60),
      ),
    ],
  );
  ```

### 4. Building a Simple UI
- **Create a Layout**:
  - Use the widgets you learned about to build a simple user interface. For example, create a basic profile card:
  
```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(title: Text('Profile Card')),
        body: Center(
          child: Container(
            width: 300,
            padding: EdgeInsets.all(16),
            decoration: BoxDecoration(
              color: Colors.white,
              border: Border.all(color: Colors.blueAccent),
              borderRadius: BorderRadius.circular(8),
            ),
            child: Column(
              children: [
                Text('John Doe', style: TextStyle(fontSize: 24)),
                SizedBox(height: 10),
                Text('Flutter Developer', style: TextStyle(color: Colors.grey)),
                SizedBox(height: 10),
                Row(
                  mainAxisAlignment: MainAxisAlignment.spaceEvenly,
                  children: [
                    Icon(Icons.mail),
                    Icon(Icons.phone),
                  ],
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

### 5. Interactivity with Stateful Widgets
- **Create a Stateful Widget**:
  - Learn how to create a widget that can change state. For example, a button that increments a counter:
  
```dart
class CounterApp extends StatefulWidget {
  @override
  _CounterAppState createState() => _CounterAppState();
}

class _CounterAppState extends State<CounterApp> {
  int _counter = 0;

  void _incrementCounter() {
    setState(() {
      _counter++;
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: Text('Counter')),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            Text('Button pressed: $_counter times'),
            ElevatedButton(
              onPressed: _incrementCounter,
              child: Text('Increment'),
            ),
          ],
        ),
      ),
    );
  }
}
```

### 6. Practice and Explore More Widgets
- **Experiment**:
  - Try different widgets and properties. Modify parameters to see how they affect the layout.
- **Explore the Flutter Widget Catalog**:
  - Visit the [Flutter Widget Catalog](https://flutter.dev/docs/development/ui/widgets) to discover more widgets.

### 7. Additional Resources
- **Flutter Documentation**: [Flutter Widgets](https://flutter.dev/docs/development/ui/widgets)
- **Flutter YouTube Channel**: Check out video tutorials about widgets and layouts.
- **Online Courses**: Consider platforms like Udemy or Coursera for structured learning.

### 8. Summary
By the end of Day 3, you should have a solid understanding of Flutter widgets, including how to create both stateless and stateful widgets. You'll also have hands-on experience building a simple user interface and using various layout widgets.
```

This expanded Day 3 plan provides detailed explanations of Flutter widgets, examples, and practical exercises. Feel free to modify any sections to better suit your learning objectives!
