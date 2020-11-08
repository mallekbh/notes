## Chapter 05: The Singleton Pattern One of a Kind Objects

- **Category:** Creational<br>

Create objets for which there is only one instance of. Many types: thread pools, caches, dialog boxes, objects that handle preferences and registry settings, objects used for logging, objects that act as device drivers to devices like printers and graphics cards, objects that act as config holders, read-only value objects, etc.

- In many ways, **the Singleton pattern** is a convention for ensuring one and only one object is instantiated for a given class. It also gives a global point of access, just like a global variable, but without the downsides. Also objects might be created only when they are needed.

### Singleton Pattern defined
**The Singleton Pattern** ensures a class has only one instance, and provides a global point of access to it.

### Dealing with multi-threading

1- **Do nothing if the performance of getInstance() isn't critical to your application:** Synchronizing getInstance() is straightforward and effective. Just keep in mind that synchronizing a method can decrease performance by a factor of 100. S of a high traffic part of your code begins using getInstance(), you may have to reconsider.

2- **Move to an eagerly created instance rather than a lazily created one:** If your application always creates and uses an instance of the Singleton or the overhead of creating and runtime aspects of the Singleton are not onerous, you may want to created your Singleton eargerly, like this:

public class Singleton {
    private static Singleton uniqueInstance = new Singleton();
    private Singleton() {}
    public static Singleton getInstance() {
        return uniqueInstance;
    }
}

Using this approach, we rely on the JVM to create the unique instance of the Singleton when the class is **loaded**. The runtime guarantees that the instance will be created before any thread acceses the static uniqueInstance variable.

    - The Singleton Pattern ensures you have at most one instance of a class in your application.
    - The Singleton Pattern also provides a global access point to that instance.
    - Java's implementation of the Singleton Pattern makes use of a pribte constructor, a static method combined with a static variable.
    - Examine your performance and resource constraints and carefully choose an appropriate Singleton implementation for multithreaded applications (and we should consider all applications multithreaded!).
    - Beware of the double-checked locking implementation; it is not thread-safe in versions before java2, version 5.
    - If you are using a JVM earlier than 1.2, you'll need to create a registry of Singletons to defeat the garbage collector.
    

    
