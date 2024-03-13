JAVA OOPs Basic
---

**Question 1: What is the main difference between an abstract class and an interface in Java?**

_Answer:_  
The main difference lies in their purpose and usage:
- **Abstract Class**:
  - Can have both abstract (unimplemented) and concrete (implemented) methods.
  - Can have member variables, constructors, and regular methods.
  - Allows code reusability by providing a common base for subclasses to extend.

- **Interface**:
  - Contains only method declarations without method bodies.
  - Cannot have member variables or constructors.
  - Defines a contract for classes to implement, facilitating multiple inheritances in Java.

**Example:**
- **Abstract Class Example**: A `Vehicle` abstract class with common methods like `move()` and `stop()`.
- **Interface Example**: An `ElectronicDevice` interface with methods like `turnOn()` and `turnOff()`.

---

**Question 2: What is the difference between a constructor and a method?**

_Answer:_  
The key differences are in their purpose and invocation:
- **Constructor**:
  - Special method called automatically when an object is instantiated.
  - Initializes the object's state, typically by setting initial values to instance variables.

- **Method**:
  - General-purpose block of code that performs a specific task when called.
  - Can manipulate data, perform operations, and return values.

**Example:**
- **Constructor Example**: `public Car(String model, int year)` initializes a `Car` object with a model and year.
- **Method Example**: `public void accelerate(int speed)` increases the speed of the car.

---

**Question 3: What is the difference between static and non-static methods?**

_Answer:_  
The distinction lies in their association with the class and objects:
- **Static Methods**:
  - Belong to the class rather than instances.
  - Can be called using the class name and cannot access instance variables.

- **Non-Static Methods**:
  - Associated with instances of the class.
  - Accessed using object references and can access instance variables.

**Example:**
- **Static Method Example**: `public static int factorial(int n)` calculates the factorial of a number.
- **Non-Static Method Example**: `public void moveForward(int distance)` moves a car forward by a given distance.

---

**Question 4: What is the difference between Inheritance and Composition?**

_Answer:_  
The distinction lies in their relationships between classes:
- **Inheritance**:
  - "Is-a" relationship where a subclass inherits from a superclass.
  - Promotes code reuse and specialization.

- **Composition**:
  - "Has-a" relationship where a class contains instances of other classes.
  - Promotes code reuse by assembling objects instead of inheriting behavior.

**Example:**
- **Inheritance Example**: A `Car` class extends a `Vehicle` class to inherit common vehicle functionalities.
- **Composition Example**: A `Car` class contains instances of `Engine`, `Wheel`, and `Body` classes.

---

**Question 5: What is the difference between overloading and overriding?**

_Answer:_  
The distinction lies in their purposes and contexts:
- **Overloading**:
  - Involves defining multiple methods with the same name but different parameters.
  - Provides different implementations based on the number or types of parameters.

- **Overriding**:
  - Involves redefining a method in a subclass that is already defined in the superclass.
  - Allows for a specialized implementation of a method in the subclass.

**Example:**
- **Overloading Example**: `calculateArea(int side)` and `calculateArea(int length, int width)` in a `Shape` class.
- **Overriding Example**: `start()` method in a `Car` subclass overrides the `start()` method in the superclass `Vehicle`.

---

**Question 6: Can you override a private or static method in Java?**

_Answer:_  
No, private methods cannot be overridden due to visibility restrictions, and static methods are not overridden but can be redefined in subclasses (method hiding).

**Example:**
- **Private Method Example**: A `Vehicle` class with a `private void startEngine()` method cannot be overridden in subclasses.
- **Static Method Example**: A `Vehicle` class with a `static void start()` method can be redefined in subclasses using method hiding.

---

**Question 7: What modifiers may be used with a top-level class?**

_Answer:_  
Top-level classes can have `public` or `default` (no modifier) access levels.

**Example:**
- **Public Top-Level Class**: `public class Car {...}`
- **Default Top-Level Class**: `class Bicycle {...}`

---

**Question 8: What is the difference between a nested public static class and a top-level class in Java?**

_Answer:_  
The distinction lies in their scope, visibility, and relationship with other classes:
- Nested Public Static Class: Defined within another class, accessible from any class using the enclosing class name.
- Top-Level Class: Stands alone, accessible independently from any other class.

**Example:**
- **Nested Public Static Class Example**: `class Car { public static class Engine {...} }`
- **Top-Level Class Example**: `public class Bicycle {...}`

---

**Question 9: What is the difference between Composition, Aggregation, and Association in OOP?**

_Answer:_  
Each represents a different level of relationship between classes:
- Composition: Strong "has-a" relationship where one class contains another class and the contained class cannot exist without the container.
- Aggregation: Weak "has-a" relationship where one class contains another class, but the contained class can exist independently.
- Association: Generic relationship between classes without implying specific ownership or dependency.

**Example:**
- **Composition Example**: A `House` class composed of `Room` objects.
- **Aggregation Example**: A `University` class aggregating `Student` objects.
- **Association Example**: A `Library` class associating with `Book` objects.

---

**Question 10: What is the difference between `this()` and `super()` in Java?**

_Answer:_  
Both are used to call constructors, but for different purposes:
- `this()` is used to call one constructor from another constructor within the same class.
- `super()` is used to call a constructor of the superclass from a subclass constructor.

**Example:**
- **`this()` Example**: `this(0)` calls another constructor within the same class.
- **`super()` Example**: `super(value)` calls the superclass constructor with a parameter.

---

This compilation provides a comprehensive overview of key concepts in Java OOP, along with real-time examples for better understanding and revision purposes.