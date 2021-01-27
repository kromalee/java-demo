# Object-Oriented

## Object

- state
- behavior

## Class

- A class is the blueprint from which individual objects are created

```java

class Bicycle {
    int cadence = 0;
    int speed = 0;
    int gear = 1;

    void changeCadence(int newValue) {
        cadence = newValue;
    }

    void changeGear(int newValue) {
        gear = newValue;
    }

    void speedUp(int increment) {
        speed = speed + increment;
    }

    void applyBrakes(int decrement) {
        speed = speed - decrement;
    }

    void printStates() {
        System.out.println("cadence:" +
                cadence + " speed:" +
                speed + " gear:" + gear);
    }
}

```

## Inheritance
- Common behavior can be defined in a superclass and inherited into a subclass

```java
class MountainBike extends Bicycle {

    // new fields and methods defining 
    // a mountain bike would go here

}
```

## Interface 
- A collection of methods with no implementation is called an interface

```java
interface Bicycle {
    void changeCadence(int newValue);

    void changeGear(int vewValue);

    void speedUp(int increment);

    void applyBreaks(int decrement);
}
```

## Package
- A namespace that organizes classes and interfaces by functionality is called a package