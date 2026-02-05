# Object-Oriented Programming

Object-Oriented Programming, also known as `OOPS`, is a programming approach that focuses on creating objects which represent real-world entities. These objects contain both data and behavior. OOPS helps manage complex systems by improving code organization and reducing dependency between components.

The `four` core principles of Object-Oriented Programming are:

* Encapsulation

* Abstraction

* Inheritance

* Polymorphism

## Encapsulation

Encapsulation is the process of wrapping `data` and `methods` together into a single unit. It restricts direct access to internal variables and ensures controlled modification of data.

### Example
```

class Employee {
    private int id;
    private String name;

    public Employee(int id, String name) {
        this.id = id;
        this.name = name;
    }

    public int getId() {
        return id;
    }

    public String getName() {
        return name;
    }
}

```

In this example, the data members are private and accessed only through public methods, which improves security and data integrity.

## Abstraction

Abstraction hides `implementation` details and exposes only essential `functionality`. It allows developers to focus on what an object does instead of how it does it.

### Example

```

interface Payment {
    void pay(double amount);
}

class CreditCardPayment implements Payment {
    public void pay(double amount) {
        System.out.println("Paid " + amount + " using Credit Card");
    }
}

```

The implementation details of payment processing are hidden from the user.

## Inheritance

Inheritance allows one class to acquire the `properties` and `behavior` of another class. It promotes code reuse and reduces duplication.

### Example

```

class Vehicle {
    void start() {
        System.out.println("Vehicle started");
    }
}

class Car extends Vehicle {
    void drive() {
        System.out.println("Car is driving");
    }
}

```

The Car class inherits the start method from the Vehicle class.

## Polymorphism

Polymorphism allows methods to behave differently based on the object that invokes them. It supports `flexibility` and `extensibility`.

### Example

```

class Shape {
    void draw() {
        System.out.println("Drawing shape");
    }
}

class Circle extends Shape {
    void draw() {
        System.out.println("Drawing circle");
    }
}

```


The correct draw method is executed at runtime depending on the object type.

### Benefits of Applying OOP in the Project

* Improves readability and structure of the code

* Makes the codebase easier to maintain

* Encourages reusability of components

* Reduces code duplication

* Simplifies testing and future enhancements

Applying Object-Oriented Programming principles during refactoring significantly improves the quality and reliability of the software.

### References

[Oracle](https://docs.oracle.com/javase/tutorial/java/concepts/)

[GeeksForGeeks](https://www.geeksforgeeks.org/object-oriented-programming-oops-concept-in-java/)

https://www.javatpoint.com/java-oops-concepts

https://www.tutorialspoint.com/java/java_object_oriented.htm
