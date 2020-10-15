Subject object manages some bits of data.<br>
The observers have subscribed to (registered with) the Subject to recieve updates when the Subject data changes.<br>
When data in the Subject changes, the Observers are notified.<br>
New data values are communicated to the observers in some form when they change.<br>

### A day in the life of the observer pattern
The subject holds an int value.<br>
The list of observers include: Dog object, Mouse object and Cat object.<br>
1- A duck object comes along and tells the Subject that it wants to become an observer.<br>
2- The subject gets a new value. All the observers are notified along with the new value communicated to them.<br>
3- The Mouse object asks to be removed.<br>
4- The subject has a new int value, observers are notified except the Mouse object.<br>

### The observer pattern defined
When you're trying to picture the Observer pattern, a newspaper subscription service with its publisher and subscribers is a good way to visualize the pattern.<br>
The conceptual definition howerver is as like this: **The Observer Pattern** defines a **One-To-Many** dependency between objects, so when one object changes state all of it's dependents are notified and updated automatically. Depending on the style of the notification the observer may also be updated with new values.

### The class diagram
![Observer Pattern Class Diagram](images/observer_class_diagram.png)
