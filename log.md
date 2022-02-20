# 100 Days Of Code - Log

### Day 41: February 20, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. SingleChildScrollView - allows scrolling on a single child widget if it gets too big for the screen.
2. ListView can be used in two different ways. ListView(children: []) and ListView.builder(). The ListView.builder() only loads/renders the items visible to the screen, optimizing performance.

**Thoughts**: 
Todays session was quite short - but better than nothing :)

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)

### Day 40: February 19, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. The commando for getting packages dependencies is `flutter pub get` not `flutter packages get`.
2. The input from a TextField is always a String.
3. Converting a string to a double: `double.parse("3.4")`
4. To track the user input on a TextField we can use the  `TextEditingController()`. Like this:
```
final titleController = TextEditingController();

TextField(
  decoration: InputDecoration(
    labelText: 'Title',
  ),
  controller: titleController,
),
```
to access the value we can use `titleController.text`.


**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)


### Day 39: February 18, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. Container: takes only one child widget, has a lot of alignment and styling options, and has a flexible width (eg. child width or available width). Containers are perfekt for custom styling and alignment.
2. Column/Rows: takes multiple child widgets, has alignment options but no styling options. A column always takes the available height, and a row takes the available width. Must-use widget that should sit next to or above each other. 
3. It's possible to combine Container and Column/Row.
4. [https://pub.dev/](https://pub.dev/): This website has all packages available for Dart and Flutter. 
5. intl is a package that can be used for e.g., translations and date formatting
6. To install a package, we need to add the package name and version under the key `dependencies` in the `pubspec.yaml` file and run `flutter pub get` to install the package. 


**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)

### Day 38: February 17, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. Column: Position widgets under each other. Main Axis is top to bottom and Cross Axis is left to right.  
2. Row: Position widgets next to each other. Main Axis is left to right, and the Cross Axis is top to bottom.

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)

### Day 37: February 16, 2022

  **Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

  **Learned**:
  1. App/Page Setup: MaterialApp or CupertinoApp and Scaffold/CupertinoPageScaffold
  Layout: Container, Row, and Column.
  2. Row/Column Children: Flexible and Expanded
  3. Content Containers: Stack, Card, 
  4. Repeat Elements: ListView, GridView, ListTile 
  5. Content Types: Text, Image, Icon
  6. User input: TextField, Buttons, GestureDetector, InkWell
  7. Flutter package manager: https://fvm.app/
  8. Create a new project with fvm installed: `fvm fluuter create projecet_name`

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)


### Day 36: February 15, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. How to install an app on an actual Android device, and not only on the emulator. 
2. How to install an app on an actual iOS device, and not only on the emulator. 
3. Syntax errors: This could be a missing semicolon or typo in a keyword. 
4. Logical errors: The code is not executed as intended. 

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)


### Day 35: February 12, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. Getter: Getters are special methods that provide read access to an object’s properties.
It's also possible to create additional properties by implementing getters, using the get and set keywords: A getter does not take any arguments and is added by using the keyword `get`:
```
class Rectangle {
  double left, top, width, height;

  Rectangle(this.left, this.top, this.width, this.height);

  // Define two calculated properties: right and bottom.
  double get right => left + width;
  set right(double value) => left = value - width;
  double get bottom => top + height;
  set bottom(double value) => top = value - height;
}
```
2. Button widgets: OutlinedButton(), TextButton(), ElevatedButton().
```
ElevatedButton(
  style: ElevatedButton.styleFrom(
    primary: Colors.orange,
    onPrimary: Colors.white,
  ),
  onPressed: () => print('Pressed Elevated button'),
  child: Text('A Raised Button'),
),
TextButton(
  child: Text("A Flat button"),
  style: TextButton.styleFrom(primary: Colors.orange),
  onPressed: () => print('Pressed Flat button'),
),
OutlinedButton(
  onPressed: () => print('Pressed Outlined button'),
  child: Text("A outlined button"),
  style: OutlinedButton.styleFrom(
    primary: Colors.orange,
    side: BorderSide(color: Colors.orange),
  ),
)
```

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)


### Day 34: February 11, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. "Lifting the state up" is a concept where you manage the state on the shared widget.
2. Splitting larger widgets into smaller widgets makes a lot of sense. 
3. a final variable can only be set  once.

**Thoughts**: 
Today's session had a lot of repetition of some concepts in Dart. 

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)

### Day 33: February 10, 2022

**Today's Progress**: I moved on with the course: "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. Container() widget. This widget always tries to be as small as possible. But it's also possible to give width and height and margin and padding.
2. Padding: Spacing inside of the container. 
3. Margin: Spacing around the container
4. Border: The border is "placed" between the padding and margin. 

Example: 
Container
Margin
Border
Padding
Child Component

5. Widget catalog: https://docs.flutter.dev/development/ui/widgets


**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)

### Day 32: February 9, 2022

**Today's Progress**: I moved on with the course "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. The setState() method calls the Build() method of the widget.
2. Private classes are written with an underscore in front of the name: _MyAppState 

**Thoughts**: Today was a short session. But better than none. 

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)


### Day 31: February 8, 2022

**Today's Progress**: I moved on with the course "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. Visible widgets: Output and input. These are visual widgets, like Buttons, Text, or Images.
2. Invisible widgets: They help control the app's layout and handle the widget tree, but they aren't visible, so they are used to layout the Visible Widgets. Examples of invisible widgets would be Row, Column, or Listview.
3. `Column()` widget: Renders widgets above each other. 
```
Column(
  children: [
    Text("The Question"),
    RaisedButton(
      child: Text("Answer"),
      onPressed: null,
    ),
  ],
);
```
4. `Row()` widget: Renders widgets next to each other. 

5. State: Data/Information used by the App.

App State:
- Authenticated Users
- Loaded jobs

Widget State:
- Current User Input
- Should a Loading Spinner be shown?

6. Stateless => Data can change externally, and the Widget gets (re)rendered when externally data changes.
7. Stateful => Data can change externally and internally, and the Widget gets (re)rendered when the externally or internally data changes.

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)

### Day 30: February 7, 2022

**Today's Progress**: I watched the course "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. Flutter is all about widgets
2. Widgets are building blocks that get rendered to the screen - like a list, app bar, or list items. 
3. Class names are written in PascalCase
4. Every widget is a Dart Class with a build() method.
5. @override is a decorator -> @override is used to show a method is overridden on purpose.  
6. Example of a hello-world app:
lib/main.dart
```
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override // Decorator
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Text("Hello!"),
    );
  }
}
```
7. The widget Scaffold() creates a basic page design. 
8. Hot reload: Injects our new code into the existing one without having to rebuild the app. 
9. Example with a Scaffold() widget. 
```
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override // Decorator
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("My first App!"),
        ),
        body: Text("This is my default text!"),
      ),
    );
  }
}
```
**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)


### Day 29: February 6, 2022

**Today's Progress**: I started the course "Flutter & Dart - The Complete Guide [2022 Edition]" by Maximilian Schwarzmüller on Udemy.

**Learned**:
1. Flutter projects should be written in snake_case, all lowercase. 
2. Folder: `android`; Holds the code for android. 
3. Folder: `ios`; Holds the code for iOs. 
4. Folder: `build`; Holds the output of the Flutter application. This folder is generated and managed by the flutter SDK. You should not add/edit anything in this folder!
5. Folder: `lib`; Libary - holds the code for the application. 
6. Folder: `test`; Holds the code for tests. 
7. File: `pubspec.yaml`: Used to manage dependencies of the project. 
8. File: `.metadata`, `.packages`, `project_name.iml` and `pubspec.yaml`; files that are automatically generated by the Flutter SDK.

**Thoughts**: 
I have done this course before, but it was almost two years ago, so I hope I will understand more this time around and that the content will be a bit easier to understand because I have already seen it once before.

**Links**:
[Learn Flutter and Dart](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)



### Day 28: February 5, 2022

**Today's Progress**: I watched the last half of the video "#22 - Dart Asynchronous Workflows - All Futures, Streams, Async Generator Functions" from `Dart - from Novice to Expert`.

**Learned**:
1. Example: 
```
void main() {
  test2Future();
}

void test2Future() {
  print("1");
  scheduleMicrotask(() => print(2));

  Future.delayed(const Duration(seconds: 1), () => print("3"));

  Future(() => print("4")).then((_) => print(5)).then((_) {
    print("6");
    scheduleMicrotask(() => print("7"));
  }).then((_) => print("8"));

  scheduleMicrotask(() => print("9"));

  Future(() => print("10"))
    .then((_) => Future(() => print('11')))
    .then((_) => print('12'));

  Future(() => print('13'));
  scheduleMicrotask(() => print('14'));
  print(15);
}

Prints
1
15
2
9
14
4
5
6
8
7
10
13
11
12
3
```
2. Keyword await. To wait for a future to complete before it assigns its value to a variable. 
```
void main() {
  late final int a;

  print("Start");

  Future(() => 1).then((value) => a = value);

  print(a);

```
  print("end");
}
=> this will through an error because a hasn't been assigned a value yet. In the future, we try to assign a value to a, but this will happen sometime in the future, and not before we are colling an int the print statement on the following line. 

Using the await keyword: 
```
void main() {
  //testFuture();
  //test2Future();

  late final int a;

  print("Start");

  Future(() => 1).then((value) => a = value);

  print(a);

  print("end");
}
```
This will pause the program until the future is resolved and we have a synchronous workflow again. 

3. .then and await togehter
```
Future main() async {
  late final int a;

  print("Start");

  await Future(() => 1).then((value) => a = value);

  print(a);

  print("end");
}
```
4. Streams -> can return 0, 1 or multiple values. 


### Day 27: February 3, 2022

**Today's Progress**: I watched the last half of the video "#22 - Dart Asynchronous Workflows - All Futures, Streams, Async Generator Functions" from `Dart - from Novice to Expert`.

**Learned**:
1. Synchronous operations: A task that needs to be solved before solving the next one. 
2. Asynchronous operations: A task that doesn't need to be solved before the next task. 
3. Futures -> Asynchronous event. 
can be: 
unprocessed (event is waiting in the event queue)
Uncompleted (processed by the event loop, but the value has not been retrieved yet. 
Completed with an expected value
completed with an error
4. Example
```
void main() {
  print("Start");

  Future(() => 1).then(print); // .then(print) => tells dart to print the returned value.
  Future(() => Future(() => 2)).then(print).onError((error, stackTrace) => null); // .onError() Can be used to catch the errors from a Future.

  Future.delayed(const Duration(seconds: 1), () => 3).then(print).whenComplete(() => null); // .whenComplete() is returns the value no matter if the value is an error or the expected value.
  Future.delayed(const Duration(seconds: 1), () => Future(() => 4)).then(print);

  Future.value(5).then(print);
  Future.value(Future(() => 6)).then(print);

  Future.sync(() => 7).then(print);
  Future.sync(() => Future(() => 8)).then(print);

  Future.microtask(() => 9).then(print);
  Future.microtask(() => Future(() => 10)).then(print);

  Future(() => 11).then(print);
  Future(() => Future(() => 12)).then(print);

  print("End");
}


prints: 
Start
End
5
7
9
1
6
8
11
10
2
12
3
4
````

### Day 26: January 31, 2022

**Today's Progress**: I watched the video "#21 - Dart Synchronous Workflows, Iterables, sync* generator functions, yield, yield*" from `Dart - from Novice to Expert`.

**Learned**:
1. Synchronous operation: A task that needs to be solved before proceeding to solve the next task. 
2. Iterable: is constructed lazily => so not the whole list is retured only the current element that is accessed
you can loop over it with the help oft his functions: `iterator(curr, nextItem())`
it doesn't need to have a specified length
Assessing an element will regenerate all items until the desired one is found.
3. Returning 1 value:
Synchronous: Type
 Asynchronous: future<Type>
4. Returning 0 or more values: 
Synchronous: iterable<Type>
 Asynchronous: stream<Type>

5. Example: 
```
void main() {    
  final a = showNormal(4);
  print(a.last);
  print(a.first);
  final b = showGenerator(4);
  print(b.last);
  print(b.first);
}

List<int> showNormal(int n) {
  print('Normal started');
  final list = <int>[];
  for (var i = 1; i <=n; i++) {
     print("i -> $i");
     list.add(i);
  }
  print('Normal endet');
  return list;
}

Iterable<int> showGenerator(int n) sync* {
  print('Generator started');
  for (var i = 1; i <=n; i++) {
    print("i -> $i");
    yield i; 
  }
  print('Generator endet');
}

prints: 
Normal started
i -> 1
i -> 2
i -> 3
i -> 4
Normal endet
4
1
Generator started
i -> 1
i -> 2
i -> 3
i -> 4
Generator endet
4
Generator started
i -> 1
1
```
6. Asynchrony => means items are generated in the background while you can process other tasks
7. Laziness => means items are generated synchronously, but only at the time, you will need them.

### Day 25: January 30, 2022

**Today's Progress**: I watched the last half of the video "#20 - Dart Isolates, Threads, The Event Loop, Microtasks, Synchronous & Asynchronous workflows" from `Dart - from Novice to Expert`.

**Learned**:
1. Synchronously => when a line of code get processed after each other, in the order. You can't move to the next step without solving the current step. 
2. Asynchronously => Allow code to proceed with other lines of code while some part of the code is taking a bit longer to finish. 
3. Everything that takes a longer time to process should be handled asynchronously so the program isn't blocked in the meantime. Examples could be network requests or storing a file. 
4. Flutter is single-threaded and runs in an isolate.
An Isolate has: 
- An event queue (only one because it's single-threaded)
- Events (every line of code)
- Event loop, with an event handler, the event handler process every line of code and blocks the program while calculating. 
- A helper thread this thread acts as a garbage collector and cleans up the code. 

5. Parallelism: Having multiple isolates, these do not use the same memory, so it's not easy to communicate between isolates. 

5. Microtasks ques: Microtasks events have a higher priority than future events. 
6. example:
```
import 'dart:math';

void main() {    
  print("#1 - squrt(4) -> ${sqrt(4)}");
  print("#2 - multiply(15*4) -> ${(15*4)}");
  print("#3 - squrt(4) -> ${50 + 10}");
  Future.delayed(const Duration(seconds: 5), () =>  print("#4 - mulitiply(4*5) -> ${4*5}"));
  print("#5 - difference(20,5) -> ${20 - 5}");
}

prints: 
#1 - squrt(4) -> 2
#2 - multiply(15*4) -> 60
#3 - squrt(4) -> 60
#5 - difference(20,5) -> 15
#4 - mulitiply(4*5) -> 20
```

### Day 24: January 27, 2022

**Today's Progress**: I watched the last half of the video "#19 - Dart Testing Explained - Unit, Integration, E2E and why you should aim for 100% code coverage" from `Dart - from Novice to Expert`.

**Learned**:
1. 100% code coverage - is when every single line of code is tested. 
2. The name of a test file should contain the name of the file's to be tested and  _test: triangle_test.dart
3. Unit tests: 
Unit tests focus on testing the smallest piece of software like function/method or a class.
4. Mock Object
Mock objects are simulated objects that can mimic the behavior of a real object lie user-actions, events and instantiate child components. 
5. Component "Widget" Tests
Tests that verify that a component behaves as expected. A component might consist of multiple classes. Objects are often mocked to test components/widgets to simulate a certain behavior. 
6. Integrations "E2E" (End-To-End) Tests
E2E Test verifies either the whole app's behavior or significant portions of the app. 

**Thoughts**: 
Defenetly have to dig deeper into tests, and how to write them in Dart. 


### Day 23: January 26, 2022

**Today's Progress**: I watched the last half of the video "#18 - Dart Libraries & Private Fields - import, export, part, part of" from `Dart - from Novice to Expert`.

**Learned**:
1. Every .dart file represent a new library in Dart
2. Every library that should be available to other Packages has to be placed in the Dart project's lib folder.
3. You can use the library keyword in a file to tell Dart that a file is a library - (this is not required because all files are libraries, and this is automatically added).
4. Private fields and methods are prefixed with a underscore. 
library first_library;
```
class A {
  final int _privateField = 5;
  void _privateMethod() {}

  final int publicField = 10;
  void publicMethod() {}
}
```
Dart only has Library private fields and not class private fields; this means that you can use private fields all over a library and not only in a specific class. 

5.  Import a library: 
```
import 'package:dart_exercise/first_library.dart';

void main() {
  var a = A();
}
```
6. Make more files into one library with the keywords part and part of
```
// File first_library.dart
library first_library;

part 'first_library_extention_1.dart';
part 'first_library_extention_2.dart';

class A {
  final int _privateField = 5;
  void _privateMethod() {}

  final int publicField = 10;
  void publicMethod() {}
}

void randomFunction() {
  var a = A();
  a._privateField;
  a.publicMethod();
}

// File first_library_extention_1.dart
part of 'first_library.dart';

void randomFunction1() {
}
```
In a file where you use the part of keyword, you can't use any import statements. Importing other libraries has to be done in the `part` file, because this is the library's root.

6.  A library can contain other libraries.  
```
// File top_library.dart 
library top_library;

export 'first_library_extention_1.dart';
export 'first_library_extention_2.dart';
```

Now you can import the whole library or only the parts like 'first_library_extention_1.dart'.

7. Rules: 
1. Declare all your libraries containing feature implementations inside the lib folder
2. Never reach in or out of the lib folder using relative imports. Use the "package" directive.
3. Inside the library, we can use the relative imports. 


**Thoughts**: 
NOOOOOO - I forgot to copy paste my content written in Grammyly from day 22 - and now its gone :(


### Day 21: January 24, 2022

**Today's Progress**: I watched the last half of the video "#16 - Dart Classes Explained II - Inheritance(extends) vs. Abstraction(implements) vs. Mixins(with)" from `Dart - from Novice to Expert`.

**Learned**:
1. Mixins. 

Mixins are used to share behaivor between one or more classes.
Mixins are regular classes with fields and methods that other classes can use. But a mixin does not have a constructor. 
Mixins can't be instantiated. 
Mixins can't be extened.
There are three ways of declaring a mixin:
normal class without a constructor:
```
class A {}
Abstract class.
abstract class A {
  void method(){}
}
Mixin keyword
mixin A {
  void method(){}
}
```
2. Use a mixin with another class by using the keyword with.

--> it works a bit like the keyword implements, but unlike implemented classes, we don't have to implement all methods when using a mixin. 
```
class Performer {
  void perform() => print("Performs!");
}

mixin Guitarist {
  void playGuitar() => print("Playing the guitar");
  void perform() => playGuitar();
}

mixin Drummer {
  void playDrums() => print("Playing the drums");
  void perform() => playDrums();
}

class Musician extends Performer with Drummer, Guitarist {
  
}

void main() {    
  Musician musician = Musician();
  musician.playDrums(); //Playing the drums
  musician.playGuitar(); //Playing the guitar
  musician.perform(); //Playing the guitar
}
```
The order of how you mixin classes matters, here the Performer is mixed in with the Drummer first, and then mixin with the Guitarist, and therefore we the perform method from the Guitarist mixin.  

3. Extension Methods

It can be used when you want to add extra functionality to a class that cant be extended. 
```
extension IntegerExtention on int {
  int get luckyNumber => 12;
  int add15() => this + 15;
}

void main() {    
  print(1.luckyNumber); // 12
  print(10.add15()); // 25
}
```
4. Prevent classes from being extended in other files by using a private constructor: 
```
class A {
  // Private constructor
  A._();
}
```
**Thoughts**: 
Extension Methods seams pretty cool.

### Day 20: January 20, 2022

**Today's Progress**: I watched half of the video "#16 - Dart Classes Explained II - Inheritance(extends) vs. Abstraction(implements) vs. Mixins(with)" from `Dart - from Novice to Expert`.

**Learned**:
1. Every class will extend from the super class called Object 

2. Inheritance --> sharing behavior from one class to another. If once class extends another --> the class that extends another class will have all fields and methods from the class it extends. A class can only extend one class.

3. The key-word `this`is for the current class. The key word `super` refers to the parent class.

4. Example: 
```
class Animal {
  final String name;
  
  Animal({required this.name});
  Animal.fromJson() : name = 'Jerry';
  
  void whatAmI() => print("I`m an animal!");
}

class Bird extends Animal {
  // Call the animal contructor
  Bird(String name) : super(name: name); 
  //Bird.fromJson(String name) : super.fromJson();
}

class Duck extends Bird {
  Duck(String name) : super(name); 
  
  @override
  void whatAmI() => print("I`m a Duck!");
}

void main() {    
  Duck duck = Duck('Munchkin');
  print(duck.name);
  duck.whatAmI();
}
```
5. Key word `Covariant`

Used to tighten a type from a superclass to a subclass. 
[Read more here](https://dart.dev/guides/language/sound-problems#the-covariant-keyword).
```
class Animal {
  final String name;
  
  Animal({required this.name});
  Animal.fromJson() : name = 'Jerry';
  
  void whatAmI() => print("I`m an animal!");
  void chase(Animal a) {}
}

class Mouse extends Animal {
  Mouse() : super(name: 'jerry');
}

class Cat extends Animal {
  Cat() : super(name: 'Tom');
  
  @override
  void chase(covariant Mouse m) {}
}
```
 6. Polymorphism 

Is achieved by overriding a method  (@override) or overloading methods with optional parameters (@overload).

7. Abstraction

Abstract classes can't be instantiated. 
--> Abstract classes
--> Abstract methods: Methods without a function body -> can only be set inside an abstract class.
--> Interfaces: Are just a contact that you will promise to implement in a class. Interfaces are created with the use of an abstract class.


8. Keyword `implements`

Forces behavior of interfaces to derived (abgeleitete) classes. One class can implement more classes.
```
abstract class UserRepositoryInterface {
  late final List<int> userList;
  
  void create();
  List<int> read();
}

class UserRepository implements UserRepositoryInterface {
  @override
  late final List<int> userList;
  
  @override
  void create() => print('Created!');
  
    @override
  List<int> read() => [1, 2, 3];
}
```
Explicit interface = Abstract class
Implicit interface = Every class
A class can extend one other class and implement as many classes as wanted.

9. External key word

Adds an abstract method to a class.
```
class Animal {
  final String name;
  
  Animal({required this.name});
  
  void whatAmI() => print("I`m an animal!");
  void chase(Animal a) {}
  
  external void doSomething();
}

class Mouse extends Animal {
  Mouse() : super(name: 'jerry');
  
  @override
  void doSomething() => print("Hallo");
}
```

**Links**: [Dart Classes Explained II - Inheritance(extends) vs. Abstraction(implements) vs. Mixins(with)](https://www.youtube.com/watch?v=OThpFGSzV1g&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=17)


### Day 19: January 19, 2022

**Today's Progress**: I watched the video "#15 - Dart Classes Explained I - All Fields, Methods, Constructors, Operators, Getters/Setters & Singleton
" from `Dart - from Novice to Expert`.

**Learned**:
1. Class
```
class A {}

void main() {    
  var a = A(); //
  var hashcode = a.hashCode;
  
  print(hashcode);
}
```

2. Instance variables (fields)

All fields inside a class have a default getter method.
All non-final and late final fields have a default setter method. (Normal final fields can't be set outside the class, only inside constructors):

final => field can only be set once.
static => field is accesed without instantiating the class
late => can be initialised later
```
class A {
  // Private field --> can't be acces outside of the field/libary
  int? _private;
  
  int? a;
  int b = 1;
  
  // Can only be set at declaration.
  final int c = 2;
  
  late int d;
  late final int e;
  // Will only be inizialized after the first time it's accessed 
  late final int f = 5;
  
  static int g = 6;
  static late int h;
  static late int i = 8;
  static late final int j;
  
  static const int k = 10;
}
```
3. Methods --> functions inside a class

The function header should have the same name as the class
Constructors do not have a return type, as the simple instantiate a class.
Static variables can't be set inside the constructor.

Initializer field inside the function body.
```
class A {
  A(
   int p,
   int a,
   int b,
   int c,
   int d,
   int e,
   int f,
  ) : this.c = c {
    _private = p;
    this.a = a;
    this.b = b;
    this.d = d;
    this.e = e;
    this.f = f;
  
  }

  int? _private;
  
  int? a;
  int b = 1;
  
  final int c;
  
  late int d;
  late final int e;
  late final int f;
  
  static int g = 6;
  static late int h;
  static late int i = 8;
  static late final int j;
  
  static const int k = 10;
}

void main() {    
  var a = A(1,2,3,4,5,6,7);
}
```
4. Initializer list 
```
 A(
   int p,
   int a,
   int b,
   int c,
   int d,
   int e,
   int f,
  ) : this.c = c,
    _private = p,
    this.a = a,
    this.b = b,
    this.d = d,
    this.e = e,
    this.f = f;
  
  
  int? _private;
  
  int? a;
  int b = 1;
  
  final int c;
  
  late int d;
  late final int e;
  late final int f;
  
  static int g = 6;
  static late int h;
  static late int i = 8;
  static late final int j;
  
  static const int k = 10;
}

void main() {    
  var a = A(1,2,3,4,5,6,7);
}
```
5. inizialise fields inside the parameter list of a constructor
```
class A {
  //! the default constructor
  A(
    this._private, {
    this.a,
    required this.b,
    required this.c,
    required this.d,
    required this.e,
    required this.f,
   });
  
  int? _private;
  
  int? a;
  int b = 1;
  
  final int c;
  
  late int d;
  late final int e;
  late final int f;
  
  static int g = 6;
  static late int h;
  static late int i = 8;
  static late final int j;
  
  static const int k = 10;
}

void main() {    
  var a = A(1, a: 2, b: 3, c: 4, d: 5, e:6, f:7);
}
```

6. Named constructors
```
class A {
  //! the default constructor
  A({
    required this.x,
    required this.y,
  });
  
  // Named constructor
  A.zero() 
    : x=0, 
      y = 0;

  // Named constructor  
  A.fromJson({required Map<String, int> json}) 
      : x = json['x']!,
        y = json['y']!;
          
  final int x;
  final int y;
  
  @override 
  String toString() => "A(x: $x, y: $y)";
}

void main() {    
  var a = A(x:6, y:7);
  print("a => $a");
  
  var aZero = A.zero();
  print("aZero => $aZero");
  
  var aFromJson = A.fromJson(json: {'x': 5, 'y': 6});
  print("aFromJson => $aFromJson");
}
```
7. Colling another constructor
```
class A {
  //! the default constructor
  A({
    required this.x,
    required this.y,
  });
          
  // Colling another constructor
  A.zeroX({required int y}) : this(x: 0, y: y);
  
  final int x;
  final int y;
  
  @override 
  String toString() => "A(x: $x, y: $y)";
}
```

8. Constant constructors
```
class Point {
  //! Const constructor only works with final fields.
  const Point({
    required this.x,
    required this.y,
  });
  
  final int x;
  final int y;
  static const Point origin = Point(x: 0, y: 0);
  
  @override 
  String toString() => "Point(x: $x, y: $y)";
}

void main() {    
  const p1 = Point(x: 1, y: 1);
  const p2 = Point(x: 1, y: 1);
  identical(p1, p2);
  print('identical(p1,p1) --> ${identical(p1, p2)}');
}
```
9. Factory constructors

Using the keyword `factory` allows you to use the return keyword. It must always return an instance of the class.
```
class Point {
  Point({
    required this.x,
    required this.y,
  });
  
  factory Point.random({required bool isPositive}) {
    return Point(x: 1, y: 2);
  }
  
  final int x;
  final int y;
  
  @override 
  String toString() => "Point(x: $x, y: $y)";
}

void main() {    
  Point p1 = Point.random(isPositive: true);
  print('$p1');
}
```
10. Singleton:

There should only be one instance of this class in the entire project. 
```
class Singleton{
  Singleton._privateConstructor();
  static final _instance = Singleton._privateConstructor();
  factory Singleton() => _instance;
}

void main() {    
  var s1 = Singleton();
  var s2 = Singleton();
  print("identical(s1, s2) --> ${identical(s1, s2)}"); // identical(s1, s2) --> true
}
```
11. Getters and Setters

Dart provides getters and setters without having to write them out. 
```
class Car {
  late int age;
  set manufacturedYear(int value) => age = 2022 - value;
}

void main() {    
  var car = Car();
  car.manufacturedYear = 2006;
  print("car.age --> ${car.age}");
}
```
12. Static methods:

Do not have access to `this` keyword, can be accessed without instantiation a class.
```
class Car {
  static test() {
    return "hallo";
  }
}

void main() {    
  print(Car.test());
}
```

**Links**: [Dart Classes Explained I - All Fields, Methods, Constructors, Operators, Getters/Setters & Singleton](https://www.youtube.com/watch?v=7rfehxYBukk&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=16)

### Day 18: January 18, 2022

**Today's Progress**: I watched the video "#14 - Dart Control Flow Statements - if/else, for, while, switch, throw, catch + ENUMS & EXCEPTIONS" from `Dart - from Novice to Expert`.

**Learned**:
1. for loop
```
void main() {  
  var list = [1,2,4,5];
  
  for (var i = 0; i < list.length; i++) {
    print(list[i]);
  }
  
  for (var item in list) {
    print(item);
  }
  
  list.forEach(print);
}
```

2. while loop, and do-while
```
void main() {  
  int i = 0;
  while(i != 5) {
    i++;
    print(i);
  }
  
  i = 0;
// will always enter the loop nomatter what condition is set.
  do {
    i++; 
    print(i);
  } while (i != 5);
}
``` 

3. break

Used to breake out of a loop.
```
void main() {  
  var list = [1,2,4,5];
  
  for (var item in list) {
    print(item);
    if (item == 2) {
      break;
    }
  }
 }
```
4. continue

Makes it possible to skip one or more iterations i a loop.
```
void main() {  
  var list = [1,2,4,5];
  
  for (var item in list) {
    if (item == 1) {
      continue;
    }
    print(item);
  }
 }
```
5. switch 
```
void main() {    
  var condition = "Sunny";
  switch (condition) {
    case "Sunny":
      print("It's sunny");
      break;
    case "Cloudy":
       print("It's cloudy");
      break;
    default:
      print("Unknown weather");
  }
 }
```
6. Enums

Is a class that is used to represent a fixed number of constant values.
```
enum Condition { sunny, cloudy, drizzly, rainy }

void main() {  
  print(Condition.rainy);
}
```
7. Assert statement
```
void main() {    
  var list = [];
  
  assert(list.isNotEmpty, 'List most not be empty!');
}
```
8. Exceptions

try, throw, catch and final
```
import 'dart:math' as math;

void main() {    
  int min = -1; 
  int max = 2;
  int zero = min + math.Random().nextInt(max-min);
  
  print("Random zero $zero");
  
  try {
    if (zero < 0) {
      throw NegativeValue(message: "Negative value");
    } else if (zero > 0) {
      throw PositiveValue(message: "Negative value");
    } 
  } on NegativeValue {
      print("The value is Negative");
  } catch(e) {
    if (e is PositiveValue) {
      print("The value is positve");
    }
  } finally {
    zero = 0;
  }
  
  if (zero == 0) {
    print('Zero at the end: $zero');
  }
}

class NegativeValue implements Exception {
  final String message;
  NegativeValue({required this.message});
}

class PositiveValue implements Exception {
  final String message;
  PositiveValue({required this.message});
}
```


### Day 17: January 17, 2022

**Today's Progress**: I watched the video "#12 - Dart Functions - Anonymous Functions, Positional & Named Parameters, Lambdas, Closures, Scope" and "#13 - Dart Operators - Everything you need to know + Comparing 2 Objects in Dart" from `Dart - from Novice to Expert`.

**Learned**:
1. Function are objects in Dart

2. How to assign a function to a variable: 
```
void main() {
  int f = first(1); // Asigns the return value from the funtion to the varialbe -  `f1` because the fuction first gets called 
  
  var f2 = first; // Asign the function to the variable f2. f2 now holds a reference to the function names first
}

int first(int a) {
  return a;
}
	
```
3. Passing functions as function arguments: 
```
void main() {  
  var functionObject = first;

  second(functionObject, 5);
}

void second(int Function(int) f, int a) {
  print(f(4));
  print(f(a));
}

int first(int a) {
  return a;
}
```
4. Arrow shorthand syntax
Can be used when you are returning a single expression
```
// Normal function declaration
int first(int a) {
  return a;
}

// Arrow shorthand syntax
int first1(int a) => a;
int first2(int a) => a.isOdd ? 1 : 0;

```
5. Anonymous functions (lambdas, closures)

```
void main() {  
  var list = ["hello", "there"].map(applyUppercaseCaseeChanges).toList();  // Using a named function.
  
  var list2 = ["hello", "there"].map((String s) {
    return s.toUpperCase();
  }).toList(); // Using a anonymous function
  
  var list3 = ["hello", "there"].map((String s) => s.toUpperCase()).toList(); // Using an anonylous function in compination with an arrow fuction because we only return a single expression.
 
}

String applyUppercaseCaseeChanges(String s) {
  return s.toUpperCase();
}
```
####Parameters:
1. Required Positional Parameters: 

The order in which the parameters are called matters, and all parameters are required.
```
void main() {  
  requiredPositional(1, 2);
}

void requiredPositional(int a, int b) => print("$a $b");
````

2. Optional Positional Parameters

The order of the parameters cant be changed, but the parameters are not required.
```
void main() {  
  optionalPositional(1);
}

void optionalPositional([int a = 5, int b = 5]) => print("$a $b");
```
3. Required Named Parameters

With name parameters, it's possible to see what parameter you set to what value, and the order of the parameters does not matter anymore.
```
void main() {  
  requiredNamed(a: 10, b: 20);
}

void requiredNamed({required int a,  required int b}) => print("$a $b");
```
4. Optional Named Parameters:

Has the advantages of Required Named Parameters, only that the parameters are not required anymore but optional. Optional named parameters need to have a default value. 
```
void main() {  
  optionalNamed(a: 10, b: 20);
}

void optionalNamed({int a = 0, int b = 0}) => print("$a $b");
````

5. It's also possible to mix required and optional named parameters: 
```
void main() {  
  optionalAndRequiredNamed(a: 10, b: 20);
}

void optionalAndRequiredNamed({required int a, int b = 0}) => print("$a $b");
```

6. You can mix Required Positional Parameters with optional positional parameters or required/optional named Parameters, but you cant mix all three of them.
```
void main() {  
  mixOfParams(10, c: 10, b: 20);
  mixOfParams2(10, 10);
}

void mixOfParams(int a, {required int c, int b = 0}) => print("$a $b $c");
void mixOfParams2(int a, [int c = 0, int b = 0]) => print("$a $b $c");
```
####Callable classes
```
void main() {  
  A()(); // first set of () makes an instance of the class, and the second pair of () calls the function
}

class A {
  void call() => print("I'm a function.");
}
```

####Expressions

1. difference between a++ and ++a
```
void main() {  
  var a = 5;
  
  // a1 = a, then a = a + 1
  // Dart first assign a to a1 and afterwords add 1 to a
  var a1 = a++;
  print(a1); // 5
  print(a); // 6
  
  // a1 = a + 1, then a2 = a
  // Dart first adds 1 to a, and then assigns a to a2
  var a2 = ++a;
  print(a2); // 7
}
```
2.  In Dart objects are only equal if they point to the same object in memory.
```
void main() {  
  int a = 2;
  int b = 2;
  print(a == b); // true
  
  var list1 = [1, 2, 3];
  var list2 = [1, 2, 3];
  print(list1 == list2); // false
    
  var list3 = const [1, 2, 3];
  var list4 = const [1, 2, 3];
  print(list3 == list4); // true
}
```
3. Type test operators

`as`Typecast 
```
import 'dart:math' as math;
void main() {  
  var list = [1, 2.0, "test", null];
  var i = list[0] as int;
  var d = list[1] as double;
  var s = list[2] as String;
  var n = list[3] as Null;
}
````

`is` true if the object has the specified type
After checking the type of an object, Dart can now access the methods of this object. 
```
void main() {  
  var list = [1, 2.0, "test", null]..forEach((element) {
    if (element is int) {
      print("$element is of in type int");
  print(element.isEven); // Accessing methods of an integer

    } else if (element is double) {
      print("$element is of in type double");
    }
  });
}
```
`is!` true if the object doesn't have the specified type

4. conditonal expression

`condition ? expr1 : expr2;`
--> if the condition is true expr1 will be evaluated if the condition is false, the second expr2 will be evaluated.

`expr1 ?? expr2;`
--> if expr1 is not null, then that expression will evaluate; otherwise expr2 will be evaluated. 


**Thoughts**: 
I think I will fall in love with named arguments - just a feeling - that knowing the order doesn't matter anymore, and you can see what params are being set to what value seems like a huge advantage. 


### Day 16: January 16, 2022

**Today's Progress**: Today, I  did exersice 6-9 from from [this](https://hackmd.io/@kuzmapetrovich/S1x90jWGP) page.

**Learned**:
1. To filter a list Dart has a methods called `where`.  
```
void main() {
  var numbers = [1, 4, 9, 16, 25, 36, 49, 64, 81, 100];

  var evenNumbers = numbers.where((element) => element % 2 == 0).toList();

  print(evenNumbers); //[4, 16, 36, 64, 100]
}
```

**Thoughts**: 
I never really wrote small programs; as I learned to code, I mostly just started to work on rather big projects - so it's fun to sit am code some small stuff while learning the syntax of Dart.

### Day 15: January 15, 2022

**Today's Progress**: Today, I started doing some exercises from [this](https://hackmd.io/@kuzmapetrovich/S1x90jWGP) page and managed to do three exercises (3, 4 and 5). 

**Learned**:
1. Learned how to set the path to the Dart SDK in IntelliJ editor: Under preferences > Language & Frameworks > Dart
2. I have Dart installed twice on my machine at the moment, once as standalone installed with Brew and once with the flutter SDK.
3. Found and used the [documentation](https://api.dart.dev/stable/1.10.1/index.html) for Dart.
4. Learned a few ways on how to find the common unique members of two lists. 

**Thoughts**: 
It was nice to do some coding today and not do any theory besides reading in the documentation from Dart to find the methods I need. 


### Day 14: January 14, 2022

**Today's Progress**: I watched the video "#11 - Dart Built-in Types - num, int, double, String, List, Set, Map & Runes" from `Dart - from Novice to Expert`.

**Learned**:

1. Cast a string into an int:

```
void main() {
  String s = '5';

  int i = int.parse(s);
  double d = double.parse(s);
  num n = num.parse(s);

  print(i);
  print(d);
  print(n);
}
```

2. Cast int to a string:

```
   int i = 5;
   String s = i.toString();
```

3. The division operator returns a double value

```
void main() {
  int a = 3;
  int b = 4;

  var c = a/b;

  print(c); // 0,75
}
```

4. Get the truncate value of a division
Truncate means returning the integer obtained by discarding any fractional part of a number.

```
void main() {
  int a = 3;
  int b = 4;

  var c = a ~/ b;

  print(c); // 0
}
```

5. String interpolation and escaping a character:

```
void main() {
  double tempature = 33.4;
  String celcius = 'celsius';
  String s = 'It\'s $tempature ${celcius.toUpperCase()}';

  print(s); // It's 33.4 CELSIUS
}
```

6. String concatenation

```
void main() {
  String a = 'Hello ';
  String b = 'World';

  print(a + b); // Hello World
}
```

6. Multiline String:

```
String s = 'Hello \n World';
print(s); //Hello
World

String s2 = '''Hello
World''';
print(s); //Hello
World
```

7. Raw String:

```
void main() {
  String s = r'Hello \n World';
  print(s); // Hello \n World
}
```

8. Unicode

```
void main() {
  String unicode = '\u{1F339}';

  print(unicode); // 🌹
}
```

9. Lists are an ordered group of objects and can contain multiple types.

```
void main() {
   List<int> i = [1, 2, 3];
   List<bool> boolieans = [true, false, true];
   List<String> s = ['Hello', 'World', '!'];
   List<A> a = [A(),A()];

   List<num> listOfIntegersAndDoubles = [2, 3.4, 4];
   List<Object> listOfIntDoubleStrinAndBooelan = [2, 3.4, 'hey', true];
   List<Object?> listOfIntDoubleStrinBooelanAndNull = [2, 3.4, 'hey', true, null];
}

class A {

}
```

To access the methods and properties of values in the list, we need to cast them to the right type.

```
void main() {
  List<Object?> complexList = [2, 3.4, 'hey', true, null];

  var intValue = complexList[0] as int;
  var doubleValue = complexList[0] as double;
  var stringValue = complexList[0] as String;
  var booleanValue = complexList[0] as bool;
  var nullValue = complexList[0] as Null;
}
```

10. Nullable lists and lists with nullable values

```
void main() {
  List<int> a = [1, 2, 3];
  List<int?> b = [1, 2, null];
  List<int>? c = [1, 2, 3];
  List<int?>? d = null;
}
```

11. Different ways to assign lists:

```
void main() {
  List<int> a = [];
  List<int> b = [1, 3, 4];
  List<int> c = List.filled(3, 3);
  List<int> d = List.empty(growable: true);
  List<int> e = List.generate(3, (index) => index);

  print(a); // []
  print(b); // [1, 3, 4]
  print(c); // [3, 3, 3]
  print(d); // []
  print(e); // [0, 1, 2]
}
```

List literals ([]) are per default growable - meaning you can add new values to the list, after initiating them.

12. Dot operater (.) and null aware dot operator (?.)
    It can be used on an object to access class fields and methods.
    The null aware dot operator only accesses a field or method if the instance is not null and otherwise returns null.

```
void main() {
  int? a = 3;
  print(a.isEven); // false
  int? b = null;
  print(b?.isEven); // null --> its like saying, if the object is not null, then run the method isEven.
}
```

13. Cascade operator (..) and null aware cascade operator (?..)
    The Cascade operator allows us to make a sequence of operations on the same object. In addition to function calls, we can also access fields on that same object.

```
void main() {
  List<int> a = [];
  a.add(1);
  a.add(0);
  print(a); // [1, 0]

  List<int> b = [];
  b..add(2)..add(3);
  print(b); // [2, 3]
}
```

If a call returns void, you can’t construct a cascade on it.

14. Spread operator (...) and null aware spread operator (...?)
    The spread operator allows us to insert multiple values into a collection.

```
void main() {
  var a = [1, 2, 3];
  var b = [1, 3, 4];
  var c = [...a, ...b];
  print(c); //[1, 2, 3, 1, 3, 4]

  var d = null;
  var e = [...a, ...?d];
  print(e);
}
```

15. Collection if

```
void main() {
  bool promoActive = true;
  var nav = [
    'Home',
    'Furniture',
    'Plants',
    if (promoActive) 'Outlet'
  ];

  print(nav);
}
```

16. Collection for

```
void main() {
 var listOfInts = [1, 2, 3];
 var listOfStrings = [
  '#0',
  for (var i in listOfInts) '#$i'
 ];
 print(listOfStrings[1] == '#1');
}
```

17. List literals are not constant by default:

```
void main() {
  var a = [1, 2, 3];
  var b = [1, 2, 3];

  print(a.hashCode); // 175652764
  print(b.hashCode); // 1012260537
}
```

But we can make them compile-time constants by using the const keyword in front of the List literal

```
void main() {
  var a = const [1, 2, 3];
  var b = const [1, 2, 3];

  print(a.hashCode); // 73544676
  print(b.hashCode); // 73544676
}
```

18. Set: Sets are a collection of unordered unique objects.

Ways to declare a set:

```
void main() {
  var set = <int>{};
  var set1 = Set();
  var set2 = {'Hey', 'World'};
  var set3 = {1, 2, 3};
  var set4 = <int>{};
}
```
Example to show what set only has unique objects:
```
void main() {
  var set = <int>{};

  set.add(1);
  set.add(3);
  set.add(3);
  set.add(2);

  print(set); //{1, 3, 2}
}
```

Sets don't have an access operator like lists (set[0]). 

18. Maps - an object that associates keys and values
Each key must be unique - qual to JSON.

```
void main() {
  var map1 = {};
  var map2 = {
    1: 1,
    2: 2, 
    3: 3,
  };
  var map3 = Map();
  Map<String, int> i = {"key": 3};
  
  // Add new entry to map
  map1.addEntries([const MapEntry(1, 2)]);
  print(map1);
  
  // use spread operator with maps
  var map4 = {...map2};
  print(map4);
  
}
```

19. Runes - a collection containing all decimal Unicode code points of a String
```
void main() {
  var runes = Runes('hello').map((e) => e.toRadixString(16).padLeft(4, '0'),).toList();
  print(runes); // [0068, 0065, 006c, 006c, 006f]
  
  String hello = '\u{0068}\u{0065}\u{006c}\u{006c}\u{006f}';
  print(hello); // hello
}
```

**Thoughts**: This was a very loong tutorial - but it's always good to get the basics right and have a second look at them. 



### Day 13: December 14, 2021

**Today's Progress**: I watched the video "#10 - Dart Variables and the differences between Late, Var, Dynamic, Final & Const
`Dart - from Novice to Expert`.

**Learned**:

1.  Files outside a lib folder are not shared with other packages.
2.  There are four types of variables in Dart. They get their names depending on where they are declared:
    Top-level: variable that isn't linked to any class or object, they are accessible from anywhere in a program
    Static: Bound to a class or object.
    `static int i = 23;`
    Instance (also called fields/properties): Bound to a class or object.
    `double j = 33.4`
    Local: Variables with a local scope, for instance, inside a function.
3.  Nonnullable variables must be initialized (to a nun-null value) before being accessed or used.
    String car; --> this won't work, as Dart assigns null to the variable, but the variable type is not nullable.
4.  Static variables: Can be accessed without instantiating the class it lives in.

```
class A {
	static int i = 4;
}
void main() {
	print(A.i); // Output 4
}
```

5. Instance variables can be left unasigned if they get assigned in the contructor.

```
class A {
  int test;
  A({required this.test});
}
void main() {
  print(A(test: 2).test); // Output 2
}
```

6. Keyword `dynamic`: variable can change variable type; the variable can be reassigned to another value of any type.
7. Keyword `var`: variable can't change type but can be reassigned to another value of the sam type.
8. Keyword `final`: variable can't change type, and variable can't be reassigned to another value.
9. Keyword `const`: variable can't change the type and can't be reassigned to another value.
10. The keyword `const` can be used for variables, constructors and objects.

**Thoughts**: I did not develop a good idea for a small program to write, so I just watched some more theory.

**Links**:
[#10 - Dart Variables and the differences between Late, Var, Dynamic, Final & Const](https://www.youtube.com/watch?v=Efaq4LvS-es&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=11)

### Day 12: December 13, 2021

**Today's Progress**: I watched the video "#9 - Understanding Null Safety in Dart - Type Promotions, Null Assertion, Late, Required" from Flutterly's `Dart - from Novice to Expert`.

**Learned**:

1. null assertion operator (!): this is used to ensure that a nullable type isn’t null. This tells Dart that your expression is safe. (Using the `!` operator will make the code unsafe if the expression actually is null at runtime).
2. modifier `late`: can be used if you know that a variable will be initialized later than instantiating the class. (This also makes your code more unsafe, if you do forget to assign a value).

**Thoughts**: Not many thoughts today - the videos from Flutterly are super good and in-depth - but I would like to do some coding soon, so maybe I should come up with a small program that I could code.

**Links**:
[#9 - Understanding Null Safety in Dart - Type Promotions, Null Assertion, Late, Required](https://www.youtube.com/watch?v=ZZ4VVlggIVk&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=10)

### Day 11: December 12, 2021

**Today's Progress**: I watched the video "#7 - All you need to know about Dart Packages and the Pub Package Manager" from Flutterly's `Dart - from Novice to Expert`.

**Learned**:

1. Immediate dependencies: Are packages that your project depends on directly.
2. Transitive dependencies: Are packages that your immediate dependency depends on.
3. Regular dependencies: Are used in the development and production phases.
4. Dev dependencies: Are only used in the development phase. These packages are ignored when building the app for production.
5. `pubspec.lock` stores the current package information that your program depends on --> check this file into git so others install the same dependencies.
6. Code that shoud be exposed in a package should be located in the lib folder.
7. How to write a package and import it into another package by referencing the path to the locale package.

```
dependencies:
  calculator:
    path: 'packages/calculator'
```

**Thoughts**: Today, I got super tired just after I started to learn. So I decided to watch the video and take a break. I then started watching the video again and implemented all the steps necessary for creating a new package and using that in my existing project.
I guess private packages are usefull if you know you have code you will use in different projects. I always wanted to do this for my nuxt.js projects but somehow never managed - so ff you know how to do it, I would love to hear from you :)

**Links**:
[#7 - All you need to know about Dart Packages and the Pub Package Manager](https://www.youtube.com/watch?v=DciQbO_97oM&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=8)

### Day 10: December 11, 2021

**Today's Progress**: Watched two videos from Flutterly's `Dart - form Novice to Expert`

**Learned**:

1. Run your dart code with arguments:
   `dart run name_of_file arg1 arg2 arg3`
2. pubspec.yaml - is a file that keeps track of all the dependencies a project or package has.
3. pubspec.lock - automatically created when running the command
   `dart pub get`. This command is responsible for getting the current package's dependencies.

**Thoughts**: The second video today was about the Dart VM - and I must say I did not understand a lot of that. But learning about pub was super. It seems to be equivalent to Composer used in the PHP world.  
Yesterday I also dug into some flutter code, an existing project, and I learned that you could assign `const` to a widget with a variable in the constructor. I guess it makes sense. It took some time until I realized what was wrong, and in the end, I should just have read the error message to the end the first time. So - reading every line in an error message can save you some time :)

**Links**:

1. [#4 - Dart Project Components - Packages, Libraries, Lint Rules & Tests](https://www.youtube.com/watch?v=XnP3--55Uqo&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=5)
2. [#5 - Running a Dart Application In-Depth! - Dart VM, Dart Isolates, JIT & AOT Compilation](https://www.youtube.com/watch?v=NoVYI94MJio&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=6)

### Day 9: December 10, 2021

**Today's Progress**: Not too much Dart today. Had to upgrade homebrew and install macOs Monterey, which took a while.

**Learned**:

1.  SDK (Software Development Kit). Collection of tools for development
2.  Run a dart program with `dart run` --> for this command to work, locate the file containing the main() function in the bin/project-name.dart file.
3.  Dart Packages are associated with the following files and folders: .dart_tool, .pacages, pubspeck.lock, pubspeck.yaml.
4.  Libraries go into the lib folder.
5.  analysis_option.yaml - helps the Dart Static Analyser by following a set of rules called linting.
6.  Test folder is for tests.
7.  The bin folder is for command line apps.
8.  Dart Packages:

- pub.dev => collection of dart pacages.
- Application Package => a package what is not uploaded to pub.dev
- Library package => a package what is uploaded to pub.dev

**Thoughts**:

**Links**:

1. [#2 - How to install the Dart SDK on Windows, Linux and MacOS](https://www.youtube.com/watch?v=WIO5iAeNaOU&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=3)
2. [#4 - Dart Project Components - Packages, Libraries, Lint Rules & Tests](https://www.youtube.com/watch?v=XnP3--55Uqo&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=5)

### Day 8: December 9, 2021

**Today's Progress**: I started the youtube track "Dart - from Novice to Expert" from Flutterly. I watched the first two videos.

**Learned**:

1.  Static type check => happens while writing code when Dart tries to compile your code. If your code isn't type-safe, your editor will show an error. And should prevent the Developer from writing the wrong types.
2.  Run time check => an extra assessment that happens when the program is running.
3.  Sound type system: Dart won't allow the code to run into an undefined state.
4.  Dynamic types. Dart won't perform type checks on dynamic types. You will have to do this yourself to avoid an exception at runtime. But at runtime Dart will infer what type the data is.

```
dynamic age = 33;
```

4. Type Inference: Types don't need to be annotated because Dart can statically infer the type. We just need to use the keyword var. Dart does this by using the static type analyzer, which I learned about in the first step.

```
var x = 5.4; //This will be of type double
```

5. Difference between the type dynamic and the keyword var:

```
void main() {
  dynamic a = 5;
  print(a.runtimeType); // int
  a = 7.0;
  print(a.runtimeType); // double
  a = 'test';
  print(a.runtimeType); // String
}

void main() {
  var a = 5;
  print(a.runtimeType); //int
  a = 7.0; // Error: A value of type 'double' can't be assigned to a variable of type 'int'
  a = 'test'; // Error: A value of type 'String' can't be assigned to a variable of type 'int'
}
```

6. Using the following: var a; without assigning a value to the variable, Dart will internally add the type dynamic to a.
7. Sound Null Safety: Sound => Dart makes Static and Runtime Checks. Null Safety: Variables can't be null unless we explicitly say they can.

**Thoughts**: Most of the content today was a repetition of concepts, but I think I now really understand what Sound Null Safety means. And it seems that the type dynamic is a bit similar to the type mixed in PHP.

**Links**:

1. [Introduction to Dart - From Novice to Expert Tutorial Series](https://www.youtube.com/watch?v=uZvoTCSsfjo&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7)
2. [#1 - Dart Language, Type System, Soundness, Type Inference, Null Safety, JIT & AOT Compilers](https://www.youtube.com/watch?v=nQRW0_Q9RFI&list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7&index=2)

### Day 7: December 8, 2021

**Today's Progress**: Today, I started watching "The Best & Most Complete Dart Course - Visualize, Learn and Practice all Dart Language Concepts!" from Flutterly on youtube

**Learned**:

1. For Mobile and Desktop, Dart uses two different compilers. Just In Time Compiler for development and an Ahead Of Time Compiler for compiling source code into machine code. Dart uses Dart Development Compiler and Dart to Javascript Compiler for the web.
2. Just in Time (JIT) Compiler only compiles the codes it needs to, and when that code is required, this is super smart during development. Because of JIT we can use hot-reload during development in Dart and Flutter.
3. Ahead Of time (AOT) Compiler compiles the entire source code into native machine code supported by the specific platform, and it does this ahead of time before the platform runs the program.

**Thoughts**: Today's Dart session was a bit short. After finishing the course I watched the last few days, I felt a bit lost and unsure what to do next. I don't think I'm ready to move over to flutter already, so I spend some time looking for good content for learning Dart. And this 8h video might do it for me.

**Links**:
[The Best & Most Complete Dart Course - Visualize, Learn and Practice all Dart Language Concepts! Chapter 1.6 Dart Compilers at 13:55 min.](https://www.youtube.com/watch?v=F3JuuYuOUK4&t=937s)

### Day 6: December 7, 2021

**Today's Progress**: Today, I kept watching "Dart Programming in 4 hours | Full beginners tutorial" on youtube from Mike Dane.

**Learned**:

1. Object-Oriented-Programming (OOP). OOP makes it possible to create custom and complex data types, like a book or person.
2. Class: A blueprint for the news data type. We should use CamelCase for class names.
   class Book {}
3. A class can have different attributes and methods.

```
class Book {
  String title;
  String author;
  int numPages;
}
```

4. Creating instances of a class => create an actual object of a class/datatype.

```
Book newBook = Book();
```

5. Contructor:

```
class Book {
  Book(String name) { // Contructor that is used to initialize a new book
   	print("This ist the contructor of ${name}");
  }
}
```

Book newBook = Book("The new book"); // newBook is an object of the blueprint Book. 6. Initialize a class attribute:

```
class Book {
 late String name;
  Book(String name) {
   	this.name = name;
  }
}
```

7. The keyword "this" refers to the current object.
8. Methods: The same as a function but placed inside a class.

```
class Student {
  late String name;
  late double gpa;

  Student(String name, double gpa) {
    this.name = name;
    this.gpa = gpa;
  }

  bool hasHonors() {
    return this.gpa >= 3.5;
  }
}
```

**Thoughts**: Okay, so the keyword new seems to be nonpresent in Dart - I might stumble over that when starting to write actual code. The constructor is just the name of the class, also pretty handy.

**Links**:
[Dart Programming in 4 hours | Full beginners tutorial](https://www.youtube.com/watch?v=5xlVP04905w)

### Day 5: December 6, 2021

**Today's Progress**: Today, I kept on watching "Dart Programming in 4 hours | Full beginners tutorial" on youtube from Mike Dane.

**Learned**:

1. Switch statements:

```
switch(operator) {
	case '+':
		print("+");
		break;
	case '-':
		print("-");
		break;
	default:
		print('Invalid operator');
}
```

2. While Loop: This is a programming structure that keeps running as long as the condition is true.

```
int i = 0;
while (i < 5) { // loop guard
  print(i);
  i++;
 }
```

3. For loop:
   for(int i = 0; i < 3; i++){
   print(i);
   }
4. For loop (for iteratables)):

```
for(int i in [2,4,4]) {
  print(i);
}
```

5.Comments:

```
// Singleline comment
/*
Multiline comment
*/
```

**Thoughts**: Today's session was a bit short. But some core concepts got introduced. I also managed to update some information on the Wiki for writers who would like to write an Interactive story to be published on the @storyways.app platform. But now work is calling!

**Links**:
[Dart Programming in 4 hours | Full beginners tutorial](https://www.youtube.com/watch?v=5xlVP04905w)

### Day 4: December 5, 2021

**Today's Progress**: Today, I kept on watching "Dart Programming in 4 hours | Full beginners tutorial" on youtube from Mike Dane.

**Learned**:

1.  If and if/else statements:

```
  if(condition){
    action
  }
```

```
  if(condition){
    action
  } else if () {
    action
  }
```

2. Operators:

```
+⇒ add
- ⇒ subtract
* ⇒ multiply
/ ⇒ divide
% ⇒ modular ⇒ 10 % 3 = 1 ⇒ 3 goes into 10 3 times, and 1 is left
&& ⇒ and
|| ⇒ or
! => negation => turns true into false, and the other way around.
```

3. Comparison Operators:

```
== ⇒ equal to
!= ⇒ not equal to
< ⇒ less than
<= ⇒ less than or equal to
> ⇒ bigger than
> = ⇒ bigger than or equal to
```

**Thoughts**: Going through the basics makes me realize how much I have learned over the last few years. So many concepts and words were just not relatable and so far from what I knew initially. It's super motivating because I can see that I have moved forward, and I get excited to expand my knowledge.

**Links**:
[Dart Programming in 4 hours | Full beginners tutorial](https://www.youtube.com/watch?v=5xlVP04905w)

### Day 3: December 4, 2021

**Today's Progress**: I moved on with watching "Dart Programming in 4 hours | Full beginners tutorial" on youtube from Mike Dane.

**Learned**:

1. Lists (called arrays in PHP): We specify what types are stored in the list by writing `<type>` after the list keyword.
   List<int> numbers = [44, 55, 4, 32];
2. Access List items with bracetnotation:
   print(numbers[0]); //44
3. Functions: Is a collection of code that can be use multiple times.
   void funcName(){} // do not return anything
4. Entrypoint of a program is the main function
   void main(){}
5. Arguments: Information that a function needs to execute.
   void funcName(String username, int age){
   print("Hi ${username}, you are ${age}");
   }
6. Return statements: We can use the keyword return in a function to give some specific information back. This information can be stored in a variable, be printed to the console, or used within another function.
7. We need to specify what type of information a function returns: int, double, String, List<int> or Map.

**Thoughts**: Arrays are called lists in Dart. Because Dart is strictly typed, it makes me wonder if there is any way to return mixed types or have arguments that are of mixed type?! But I guess not - otherwise, it wouldn't be strict, right?! :)

### Day 2: December 3, 2021

**Today's Progress**:
Got to interact with user input in the terminal and read a lot about "Sound null safty".

**Learned**:

1. To read user input in the terminal - with stdin.readLineSync();
2. Importing statements:
   import "dart:io";
3. "Sound null safety": You explicitly have to say that a variable can be null if you want it to be null, and because Dart's null safety is sound (stable), the compiler is also optimized.

**Thoughts**: Null safety seems handy, but I think I have to dig a bit deeper into the topic to understand the fact that Dart’s null safety is sound.

**Links**:
[Dart Programming in 4 hours | Full beginners tutorial](https://www.youtube.com/watch?v=5xlVP04905w)

[Null safety](https://dart.dev/null-safety)

[Artikel about Null safety](https://www.infoworld.com/article/3562572/google-dart-gains-sound-null-safety.html)

[Artikel about Null safety in German](https://tech-de.netlify.app/articles/de513466/index.html)

[Video about Null safety](https://www.youtube.com/watch?v=iYhOU9AuaFs)

### Day 1: December 2, 2021

**Today's Progress**: I started to watch "Dart Programming in 4 hours | Full beginners tutorial" on youtube from Mike Dane.

**Learned**:

1. Print statement: print("Hello World!").
2. Execution flow of the program - From top to bottom
3. Variables: Containers that can store values.
4. Strings
5. Stringinterpolation - Insert a variable into a string: "Hello ${varName}"
6. Numbers: integer (10) and doubles (10,80)
7. Booleans: can be true or false
8. Comments: //
9. The length of a String is always one more than the last index position. Example:
   String greeting = "Hello"; //has indexes 01234
   print(greeting.length); //will print 5
   print(greeting[0]); //will print H
10. Concatination: varName + varName

Example Variables:
String firstName = "Mallle";
int age = 32;
double height = 1,72;
bool isHappy = true;

**Thoughts**:
Variables need a type - unlike in javascript. So need to get more consistent in that regard.

**Links**:
[Dart Programming in 4 hours | Full beginners tutorial](https://www.youtube.com/watch?v=5xlVP04905w)

### Day 0: December 1, 2021

**Today's Progress**:
Forked the 100daysofcode repo, watched the introduction to what Flutter is and why to use Flutter.

**Learned**:

1. Flutter uses Dart.
2. Flutter has a simple and flexible layout system that was inspired by the web and includes: Row, Column, Stack, Padding, and Center.
3. Flutter is Open Source, and you can dig into the code and see how the Flutter team implemented different widgets.
4. Flutter offers you one codebase for iOs, Android, Web, and Desktop.
5. Flutter has implemented Hot Reload - means the screen will update within fractions of a second after saving the code.

**Thoughts**:
Looking forward to writing the first lines of code and digging deeper into Dart and Flutter. It might be helpful to learn more about Dart before continuing with Flutter, as Flutter uses Dart.

**Link to work**:
[100 days of code](https://www.100daysofcode.com/)
[Introduction to Flutter Development Using Dart](https://www.appbrewery.co/p/intro-to-flutter)
