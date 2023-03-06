---
theme: /Users/hamed/Documents/Hamed/slides_0.5.0/theme.json
author: Hamed
date: MMMM YYYY
paging: slide %d | %d
---

```
 _____ _     _           _     _____      _            _           _  ______                                              _
|  _  | |   (_)         | |   |  _  |    (_)          | |         | | | ___ \                                            (_)
| | | | |__  _  ___  ___| |_  | | | |_ __ _  ___ _ __ | |_ ___  __| | | |_/ / __ ___   __ _ _ __ __ _ _ __ ___  _ __ ___  _ _ __   __ _
| | | | '_ \| |/ _ \/ __| __| | | | | '__| |/ _ \ '_ \| __/ _ \/ _` | |  __/ '__/ _ \ / _` | '__/ _` | '_ ` _ \| '_ ` _ \| | '_ \ / _` |
\ \_/ / |_) | |  __/ (__| |_  \ \_/ / |  | |  __/ | | | ||  __/ (_| | | |  | | | (_) | (_| | | | (_| | | | | | | | | | | | | | | | (_| |
 \___/|_.__/| |\___|\___|\__|  \___/|_|  |_|\___|_| |_|\__\___|\__,_| \_|  |_|  \___/ \__, |_|  \__,_|_| |_| |_|_| |_| |_|_|_| |_|\__, |
           _/ |                                                                        __/ |                                       __/ |
          |__/                                                                        |___/                                       |___/
______       _ _     _ _              ______      _               _                     _   _____           _       _     _         ___
| ___ \     (_) |   | (_)             | ___ \    | |             | |                   | | /  ___|         | |     | |   | |       / _ \
| |_/ /_   _ _| | __| |_ _ __   __ _  | |_/ /___ | |__  _   _ ___| |_    __ _ _ __   __| | \ `--.  ___ __ _| | __ _| |__ | | ___  / /_\ \_ __  _ __  ___
| ___ \ | | | | |/ _` | | '_ \ / _` | |    // _ \| '_ \| | | / __| __|  / _` | '_ \ / _` |  `--. \/ __/ _` | |/ _` | '_ \| |/ _ \ |  _  | '_ \| '_ \/ __|
| |_/ / |_| | | | (_| | | | | | (_| | | |\ \ (_) | |_) | |_| \__ \ |_  | (_| | | | | (_| | /\__/ / (_| (_| | | (_| | |_) | |  __/ | | | | |_) | |_) \__ \
\____/ \__,_|_|_|\__,_|_|_| |_|\__, | \_| \_\___/|_.__/ \__,_|___/\__|  \__,_|_| |_|\__,_| \____/ \___\__,_|_|\__,_|_.__/|_|\___| \_| |_/ .__/| .__/|___/
                                __/ |                                                                                                   | |   | |
                               |___/                                                                                                    |_|   |_|
```

---

##### Outline

# Introduction to Object Oriented Programming (OOP)

## Benefits of OOP in Dart Development

## Best Practices for OOP in Dart Development

## Conclusion

---

##### Outline

## Introduction to Object Oriented Programming (OOP)

# Benefits of OOP in Dart Development

## Best Practices for OOP in Dart Development

## Conclusion

---

##### Outline

## Introduction to Object Oriented Programming (OOP)

## Benefits of OOP in Dart Development

# Best Practices for OOP in Dart Development

## Conclusion

---

##### Outline

## Introduction to Object Oriented Programming (OOP)

## Benefits of OOP in Dart Development

## Best Practices for OOP in Dart Development

# Conclusion

---

##### Introduction to Object Oriented Programming (OOP)

## Object Oriented Programming (OOP) is a programming paradigm that focuses on using objects to represent real-world concepts.

## In OOP, objects are created from classes, which define their properties and behavior.

## This allows for the creation of modular, reusable, and scalable code, making it easier to build software that is flexible and adaptable to changing requirements.

---

##### Introduction to Object Oriented Programming (OOP)

# Object Oriented Programming (OOP) is a programming paradigm that focuses on using objects to represent real-world concepts.

## In OOP, objects are created from classes, which define their properties and behavior.

## This allows for the creation of modular, reusable, and scalable code, making it easier to build software that is flexible and adaptable to changing requirements.

---

##### Introduction to Object Oriented Programming (OOP)

## Object Oriented Programming (OOP) is a programming paradigm that focuses on using objects to represent real-world concepts.

# In OOP, objects are created from classes, which define their properties and behavior.

## This allows for the creation of modular, reusable, and scalable code, making it easier to build software that is flexible and adaptable to changing requirements.

---

##### Introduction to Object Oriented Programming (OOP)

## Object Oriented Programming (OOP) is a programming paradigm that focuses on using objects to represent real-world concepts.

## In OOP, objects are created from classes, which define their properties and behavior.

# This allows for the creation of modular, reusable, and scalable code, making it easier to build software that is flexible and adaptable to changing requirements.

---

##### Fundamental Concepts of OOP

# Attributes: A variable that is defined within a class.

```dart
String name = "John Doe";
int age = 30;
double height = 1.75;
bool isMarried = false;
```

---

##### Fundamental Concepts of OOP

# Attributes: A variable that is defined within a class.

# Methods: A function that is defined within a class.

```dart
int add(int num1, int num2) {
    return num1 + num2;
}
```

---

##### Fundamental Concepts of OOP

# Attributes: A variable that is defined within a class.

# Methods: A function that is defined within a class.

# Classes: A blueprint for creating objects.

```dart
class Person {
  String name;
  int age;

  Person(this.name, this.age);

  void sayHello() {
    print("Hello, my name is $name and I am $age years old.");
  }
}
```

---

##### Fundamental Concepts of OOP

# Attributes: A variable that is defined within a class.

# Methods: A function that is defined within a class.

# Classes: A blueprint for creating objects.

# Objects: An instance of a class.

```dart
var person1 = Person("John Doe", 30);
var person2 = Person("Jane Smith", 25);
```

---

# Encapsulation: The process of hiding the implementation details of a class from other objects.

---

# Encapsulation: The process of hiding the implementation details of a class from other objects.

```dart
class Person {
  String _name;
  int _age;
}
```

---

# Encapsulation: The process of hiding the implementation details of a class from other objects.

```dart
class Person {
  String _name;
  int _age;

  String get name => _name;
  set name(String name) => _name = name;

  int get age => _age;
  set age(int age) => _age = age;
}
```

---

# Encapsulation: The process of hiding the implementation details of a class from other objects.

```dart
class Person {
  String _name;
  int _age;

  String get name => _name;
  set name(String name) => _name = name;

  int get age => _age;
  set age(int age) => _age = age;

  void introduce() {
    print("Hi, my name is ${_name} and I am ${_age} years old.");
  }
}
```

---

# Inheritance: The process of creating a new class from an existing class.

---

# Inheritance: The process of creating a new class from an existing class.

```dart
class Vehicle {
  int numberOfWheels;
  String color;

  void start() {
    print("Starting vehicle...");
  }

  void stop() {
    print("Stopping vehicle...");
  }
}
```

---

# Inheritance: The process of creating a new class from an existing class.

```dart
class Vehicle {
  int numberOfWheels;
  String color;

  void start() {
    print("Starting vehicle...");
  }

  void stop() {
    print("Stopping vehicle...");
  }
}

class Car extends Vehicle {
  String model;

  void accelerate() {
    print("Accelerating car...");
  }

  void brake() {
    print("Braking car...");
  }
}
```

---

# Polymorphism: The ability of an object to take on many forms.

---

# Polymorphism: The ability of an object to take on many forms.

```dart
class Animal {
  void makeSound() {
    print("The animal makes a sound.");
  }
}

```

---

# Polymorphism: The ability of an object to take on many forms.

```dart
class Animal {
  void makeSound() {
    print("The animal makes a sound.");
  }
}

class Cat extends Animal {
  void makeSound() {
    print("The cat meows.");
  }
}

```

---

# Polymorphism: The ability of an object to take on many forms.

```dart
class Animal {
  void makeSound() {
    print("The animal makes a sound.");
  }
}

class Cat extends Animal {
  void makeSound() {
    print("The cat meows.");
  }
}

class Dog extends Animal {
  void makeSound() {
    print("The dog barks.");
  }
}
```

---

# Abstraction: The process of hiding the implementation details of a class from other objects.

---

# Abstraction: The process of hiding the implementation details of a class from other objects.

```dart
abstract class Shape {
  double getArea();
}

```

---

# Abstraction: The process of hiding the implementation details of a class from other objects.

```dart
abstract class Shape {
  double getArea();
}

class Rectangle extends Shape {
  double width;
  double height;

  double getArea() {
    return width * height;
  }
}
```

---

# Abstraction: The process of hiding the implementation details of a class from other objects.

```dart
abstract class Shape {
  double getArea();
}

class Rectangle extends Shape {
  double width;
  double height;

  double getArea() {
    return width * height;
  }
}

class Circle extends Shape {
  double radius;

  double getArea() {
    return 3.14 * radius * radius;
  }
}
```

---

# Benefits of OOP in Dart Development

---

# Reusability

OOP encourages the creation of modular, reusable code, making it easier to avoid duplication of code and increase efficiency.

```dart
class Calculator {
  int add(int a, int b) {
    return a + b;
  }
}
```

---

# Maintainability

OOP helps in creating code that is easy to maintain and update. By encapsulating implementation details, it becomes easier to modify and update objects without affecting other parts of the app.

```dart
class Person {
  String _name;
  int _age;

  String get name => _name;
  set name(String name) => _name = name;

  int get age => _age;
  set age(int age) => _age = age;

  void introduce() {
    print("Hi, my name is ${_name} and I am ${_age} years old.");
  }
}
```

---

# Scalability

OOP makes it easier to build software that is flexible and adaptable to changing requirements.

```dart
class Product {
  String _name;
  double _price;

  Product(this._name, this._price);

  String get name => _name;

  double get price => _price;
}

class ShoppingCart {
  List<Product> _items = [];

  void addItem(Product item) {
    _items.add(item);
  }

  double get total => _items.fold(0, (total, item) => total + item.price);
}
```

---

# Best Practices for OOP in Dart Development

## Use encapsulation:

Keep data hidden from the outside world by making variables private and providing public getters and setters.

## Follow the single responsibility principle:

Each class should have one and only one responsibility. If a class has too many responsibilities, consider splitting it into smaller classes.

## Use abstract classes to define contracts:

Abstract classes provide a way to define a contract that classes can implement or extend. This can help to reduce coupling and make code more flexible and reusable.

---

# Conclusion

OOP is an essential part of building robust and scalable apps in Flutter.

By mastering OOP concepts and best practices, developers can write high-quality code that is built to last and can be easily maintained and scaled over time.

---

```
           _   _ __     __   ____   _    _  ______   _____  _______  _____  ____   _   _  ___
    /\    | \ | |\ \   / /  / __ \ | |  | ||  ____| / ____||__   __||_   _|/ __ \ | \ | | |__ \
   /  \   |  \| | \ \_/ /  | |  | || |  | || |__   | (___     | |     | | | |  | ||  \| |   ) |
  / /\ \  | . . |  \   /   | |  | || |  | ||  __|   \___ \    | |     | | | |  | || . . |  / /
 / ____ \ | |\  |   | |    | |__| || |__| || |____  ____) |   | |    _| |_| |__| || |\  | |_|
/_/    \_\|_| \_|   |_|     \___\_\ \____/ |______||_____/    |_|   |_____|\____/ |_| \_| (_)

```
