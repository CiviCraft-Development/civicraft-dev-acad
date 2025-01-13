These are my notes on what I want to add. I need to flesh them out better.

Java is a case-sensitive language. It's keywords are written on lowercase and must always be used that way.

Java ignores spaces, tabs, new lines, and other whitespace unless it occurs in a quoted characters & string literals

Doc comments are used by javadoc to extract information

Reserved words:
* abstract
* assert
* boolean
* break
* byte
* case
* catch
* char
* class
* const
* continue
* default
* do
* double
* else
* enum
* extends
* false
* final
* finally
* float
* for
* goto
* if
* implements
* import
* instanceof
* int
* interface
* long
* native
* new
* null
* package
* private
* protected
* public
* return
* short
* static
* strictfp
* super
* switch
* synchronized
* this
* throw
* throws
* transient
* true
* try
* void
* volatile
* while

Identifiers are names giving to a class, method, variable, etc. May be any length and any letter/digit from all Unicode characters. Identifiers can include, but not start with a digit. Identifiers can't have punctuation characters. Exceptions to this: $ (us dollar), ¥ (yen), £ (pound)

Camel case is the identifier naming convention. First letter is lower case, following words begin with a capital. thisIsAnExample

Literals include integer & floating-point numbers, single characters within single quotes, strings of characters within double quotes, and the words true, false, and null. 

Java uses punctuation characters as tokens
Divided into separators and operators.

Separators: () {} [] ... @ :: ; , .

Operators: + - * / % & | ^ << >> >>> += -= *= /= %= &= |= ^= <<= >>= >>>= = == != < <= > >= ! ~ && || ++ -- ? : ->

Primitive data types: boolean, char, byte, short, int, long, float, double

Escape characters
* \b - Backspace
* \t - Horizontal tab
* \n - Newline
* \f - From feed
* \r - Carriage return
* \" - Double quote
* \' - Single quote
* \\\ - Backslash
2 others \xxx and \uxxxx but I need to learn more about them.

Special operators
* . - Member access. Members are the data and methods of an object. 
* [] - Array element access. References an element in an array based on an index.
* () - Method invocation. Runs the accessed method 
* () - Type casting. Completely different use than method invocation. 
* -> - Lambda expression. Essentially a method body. Method argument list followed by the lambda arrow which is then followed by a block of code. 
* new - Object or Array creation. Followed by the type of the object.

Java Statements are basic units of execution. 
* Expression statement - Assignment, assignment w/ operation, increment and decrement, method calls, and object creation
* Compound statement - Statements grouped together with curly braces.
* Empty statement - Statement written with a single semicolon.
* Labeled statement
* Local variable declaration statements

Method - named sequence of statements that can be invoked elsewhere

Method signature - Unique identifier for a method in a class that defines the method's input and output. Specifies:
* Method name
* Number, order, type, and name of the parameters used by the method
* The type of value returned by the method
* The exceptions the method can throw 
* Various method modifiers

modifiers type name (params) throws exception

Signature is followed by implementation

Modifiers:
* abstract - Specification w/o implementation. No code body!
* final - Cannot be overriden or hidden. Private methods are implied to be final
* native - Method implementation is written in a native language like C. No body
* public - Access modifier. Can be used outside class.
* protected - Access modifier. 
* private - Access modifier. Cannot be used outside class.
* static - Class method associated with the class itself, not the instance of the class
* strictfp - FP = Floating point, 
* synchronized - Makes method threadsafe 

Checked exception - Checked at compile time, must be handled explicitly
Unchecked exception - Checked at runtime, does not require explicit handling at compile time

type specifies the return type of the message. If the method doesn't return a value, the type should be `void`

constructor - block of code used to initialize newly created objects

