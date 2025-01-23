# Comments
Comments are text annotations within source code that are ignored by the compiler. They are used to add additional information to the written code.

## Single-Line Comments
Single-line comments begin with two forward slashes `//`. Any text that comes after these two slashes is ignored and does not impact the code in any way.

`// This is a comment`

`println("Minecraft") // This is a comment`


## Multi-Line Comments
Multi-line comments span over multiple lines. The start of it begins with `/*` and ends with `*/`.

## Documentation Comments
**KDoc** is a language used to document Kotlin code, the equivalent of Java's Javadoc. These comments begin with `/**` and end with `*/`. Each line in between these markers must begin with an asterisk. 

```
/**
 * Represents a group of members.
 *
 * This is a simple example for KDoc documentation.
 *
 * @param T The type of a member in this group.
 * @property name The group's name.
 * @constructor Creates a group with a name.
 */
class Group<T>(val name: String) {
    /**
     * Adds a member to the group.
     * @return The new group size.
     */
    fun add(member: T): Int {
        // Implementation here
    }
}
```
### KDoc Block Tags
| **Tag**              | **Description**                                    | **Example**                                       |
|----------------------|----------------------------------------------------|---------------------------------------------------|
| `@param name`        | Describes a parameter.                             | `@param name Description.`                        |
| `@return`            | Documents the return value of a function.          | `@return The size of the group.`                  |
| `@constructor`       | Details the primary constructor of a class.        | `@constructor Creates a group with a name.`       |
| `@receiver`          | Documents the receiver in an extension function.   | `@receiver The receiver of the extension.`        |
| `@property name`     | Describes a property from the primary constructor. | `@property name The group's name.`                |
| `@throws class`      | Explains exceptions that might be thrown.          | `@throws IOException If file access fails.`       |
| `@exception class`   | Same as `@throws`, for documenting exceptions.     | `@exception IllegalArgumentException If invalid.` |
| `@sample identifier` | Embeds a function body as an example.              | `@sample my.package.exampleFunction`              |
| `@see identifier`    | Adds a reference to related elements.              | `@see kotlin.collections.List`                    |
| `@author`            | Specifies the author.                              | `@author Jane Doe`                                |
| `@since`             | Marks the version of introduction.                 | `@since 1.0`                                      |
| `@suppress`          | Excludes an element from documentation.            | `@suppress This element is not public.`           |