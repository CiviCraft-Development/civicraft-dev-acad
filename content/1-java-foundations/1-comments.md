# Comments
Comments are text annotations within source code that are ignored by the compiler. They are used to add additional information to the written code.

## Single-Line Comments
Single-line comments begin with two forward slashes `//`. Any text that comes after these two slashes is ignored and does not impact the code in any way.

```java
// This is a comment
System.out.println("Minecraft"); // This is a comment
```

## Multi-Line Comments
Multi-line comments span over multiple lines. The start of it begins with `/*` and ends with `*/`.
```java
/*
This is a multi-line comment.
It can span multiple lines.
*/
```

## Documentation Comments
Javadoc is a language used to document Java code. These comments begin with `/**` and end with `*/`. Each line in between these markers can begin with an asterisk, but it is not required.

```java
/**
* Represents a group of members.
*
* This is a simple example for Javadoc documentation.
*
* @param <T> The type of a member in this group.
  */
  class Group<T> {
  /**
    * The group's name.
      */
      private String name;

  /**
    * Creates a group with a name.
    *
    * @param name The group's name.
      */
      public Group(String name) {
        this.name = name;
      }

  /**
    * Adds a member to the group.
    *
    * @param member The member to add.
    * @return The new group size.
      */
      public int add(T member) {
         // Implementation here
         return 0; // Placeholder return value
        }
      }
 ```

### Javadoc Block Tags
| **Tag**                       | **Description**                                | **Example**                                                  |
|-------------------------------|------------------------------------------------|--------------------------------------------------------------|
| `@param <var>name</var>`      | Describes a parameter.                         | `@param <var>name</var> Description.`                        |
| `@return`                     | Documents the return value of a function.      | `@return The size of the group.`                             | 
| `@throws <var>class</var>`    | Explains exceptions that might be thrown.      | `@throws <var>IOException</var> If file access fails.`       | 
| `@exception <var>class</var>` | Same as `@throws`, for documenting exceptions. | `@exception <var>IllegalArgumentException</var> If invalid.` |
| `@see <var>identifier</var>`  | Adds a reference to related elements.          | `@see java.util.List`                                        |
| `@author`                     | Specifies the author.                          | `@author Jane Doe`                                           |
| `@since`                      | Marks the version of introduction.             | `@since 1.0`                                                 |
| `@deprecated`                 | Marks an element as deprecated.                | `@deprecated Use {@link #newMethod()} instead.`              |
| `@version`                    | Specifies the version of the software.         | `@version 1.2.3`                                             |
| `@serial`                     | Used for serialization documentation.          | `@serial description`                                        |
| `@serialField`                | Documents a field in a serializable class.     | `@serialField <var>name</var> <var>type</var> description`   |
| `@serialData`                 | Documents the data written by serialization.   | `@serialData description`                                    |