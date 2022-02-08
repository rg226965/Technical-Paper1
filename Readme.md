<!--headings-->

# Collections in Java

The Collection in Java is a framework that provides an architecture to store and manipulate the group of objects.

Java Collections can achieve all the operations that you perform on a data such as searching, sorting, insertion, manipulation, and deletion.

Java Collection means a single unit of objects. Java Collection framework provides many interfaces (Set, List, Queue, Deque) and classes (ArrayList, Vector, LinkedList, PriorityQueue, HashSet, LinkedHashSet, TreeSet).

### \>What is Collection in Java
___
A Collection represents a single unit of objects, i.e., a group.

### \>What is a framework in Java
___
- It provides readymade architecture.


- It represents a set of classes and interfaces.
- It is optional.

### \>What is Collection framework
___
The Collection framework represents a unified architecture for storing and manipulating a group of objects. It has:

1. Interfaces and its implementations, i.e., classes


2. Algorithm

### \>Hierarchy of Collection Framework
___
Let us see the hierarchy of Collection framework. The java.util package contains all the classes and interfaces for the Collection framework.

![Hierarchy of Collection Framework](https://static.javatpoint.com/images/java-collection-hierarchy.png "Collection Framework hierarchy")

### \>Methods of Collection interface
___
There are many methods declared in the Collection interface. They are as follows:

| NO. | Method | Description |
| --- | --- | --- |
|1|public boolean add(E e)|It is used to insert an element in this collection.|
|2|public boolean addAll(Collection<? extends E> c)|It is used to insert the specified collection elements in the invoking collection.|
|3|public boolean remove(Object element)|It is used to delete an element from the collection.|
|4|	public boolean removeAll(Collection<?> c)|It is used to delete all the elements of the specified collection from the invoking collection.|
|5|default boolean removeIf(Predicate<? super E> filter)|It is used to delete all the elements of the collection that satisfy the specified predicate.|
|6|public boolean retainAll(Collection<?> c)|It is used to delete all the elements of invoking collection except the specified collection.|
|7|public int size()|It returns the total number of elements in the collection.|
|8|public void clear()|It removes the total number of elements from the collection.|
|9|	public boolean contains(Object element)|It is used to search an element.|
|10|public boolean containsAll(Collection<?> c)|It is used to search the specified collection in the collection.|
|11|public Iterator iterator()|	It returns an iterator.|
|12|public Object[] toArray()|It converts collection into array.|
|13|public <T> T[] toArray(T[] a)|It converts collection into array. Here, the runtime type of the returned array is that of the specified array.|
|14|public boolean isEmpty()|It checks if collection is empty.|
|15|default Stream<E> parallelStream()|It returns a possibly parallel Stream with the collection as its source.|
|16|default Stream<E> stream()|It returns a sequential Stream with the collection as its source.|
|17|default Spliterator<E> spliterator()|It generates a Spliterator over the specified elements in the collection.|
|18|public boolean equals(Object element)|It matches two collections.|
|19|public int hashCode()|It returns the hash code number of the collection.|


### \>Java Collection Interface
___

The `Collection` interface is the root interface of the collections framework hierarchy.

Java does not provide direct implementations of the `Collection` interface but provides implementations of its subinterfaces like `List`, `Set`, and `Queue`.

### \>Collections Framework Vs. Collection Interface
___
People often get confused between the collections framework and `Collection` Interface.

The `Collection` interface is the root interface of the collections framework. The framework includes other interfaces as well: `Map` and `Iterator`. These interfaces may also have subinterfaces.

### \>Subinterfaces of the Collection Interface
___
As mentioned earlier, the `Collection` interface includes subinterfaces that are implemented by Java classes.

All the methods of the `Collection` interface are also present in its subinterfaces.

Here are the subinterfaces of the `Collection` Interface:

 #### **List Interface :**
The `List` interface is an ordered collection that allows us to add and remove elements like an array.  

#### **Set Interface :**
The `Set` interface allows us to store elements in different sets similar to the set in mathematics. It cannot have duplicate elements.

#### **Queue Interface :**
The `Queue` interface is used when we want to store and access elements in First In, First Out manner.   

### \>Java Map Interface
___
In Java, the `Map` interface allows elements to be stored in key/value pairs. Keys are unique names that can be used to access a particular element in a map. And, each key has a single value associated with it.

### \>Java Iterator Interface
___
In Java, the `Iterator` interface provides methods that can be used to access elements of collections.

### \>Why the Collections Framework?
___
The Java collections framework provides various data structures and algorithms that can be used directly. This has two main advantages:
+ We do not have to write code to implement these data structures and algorithms manually.
+ Our code will be much more efficient as the collections framework is highly optimized.

Moreover, the collections framework allows us to use a specific data structure for a particular type of data. Here are a few examples,
+ If we want our data to be unique, then we can use the `Set` interface provided by the collections framework.
+ To store data in key/value pairs, we can use the `Map` interface.
+ The `ArrayList` class provides the functionality of resizable arrays.

### \>Example: ArrayList Class of Collections
___
The `ArrayList` class allows us to create resizable arrays. The class implements the `List` interface (which is a subinterface of the `Collection` interface).

```java
// The Collections framework is defined in the java.util package
import java.util.ArrayList;

class Main {
    public static void main(String[] args){
        ArrayList<String> animals = new ArrayList<>();
        // Add elements
        animals.add("Dog");
        animals.add("Cat");
        animals.add("Horse");

        System.out.println("ArrayList: " + animals);
    }
}
``` 
**Output**
```
ArrayList: [Dog, Cat, Horse]
```

### \>References :
___
+ https://www.javatpoint.com/collections-in-java
+ https://www.programiz.com/java-programming/collections