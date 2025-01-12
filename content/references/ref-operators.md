# Operators

## Arithmetic Operators
| Operator | Description           | Example           |
|----------|-----------------------|-------------------|
| +        | Addition              | int sum = a + b;  |
| -        | Subtraction           | int diff = a - b; |
| *        | Multiplication        | int prod = a * b; |
| /        | Division              | int quot = a / b; |
| %        | Modulus (remainder)   | int rem = a % b;  |

## Unary Operators
| Operator | Description            | Example               |
|----------|------------------------|-----------------------|
| +        | Unary plus (no effect) | int val = +a;         |
| -        | Unary minus (negation) | int neg = -a;         |
| ++       | Increment by 1         | x++; or ++x;          |
| --       | Decrement by 1         | x--; or --x;          |
| !        | Logical NOT            | boolean flag = !true; |

## Assignment Operators
| Operator | Description                 | Example           |
|----------|-----------------------------|-------------------|
| =        | Assign a value              | a = b;            |
| +=       | Add and assign              | a += b;           |
| -=       | Subtract and assign         | a -= b;           |
| *=       | Multiply and assign         | a *= b;           |
| /=       | Divide and assign           | a /= b;           |
| %=       | Modulus and assign          | a %= b;           |

## Relational Operators
| Operator | Description              | Example     |
|----------|--------------------------|-------------|
| ==       | Equal to                 | if (a == b) |
| !=       | Not equal to             | if (a != b) |
| <        | Less than                | if (a < b)  |
| \>       | Greater than             | if (a > b)  |
| <=       | Less than or equal to    | if (a <= b) |
| \>=      | Greater than or equal to | if (a >= b) |

## Logical Operators
| Operator | Description | Example                            |
|----------|-------------|------------------------------------|
| &&       | Logical AND | if (a > 0 && b > 0)                |
| \|\|     | Logical OR  | if (a > 0             \| \| b > 0) |
| !        | Logical NOT | boolean flag = !true;              |

## Bitwise Operators
| Operator | Description          | Example               |
|----------|----------------------|-----------------------|
| &        | Bitwise AND          | int result = a & b;   |
| \|       | Bitwise OR           | int result = a \| b;  |
| ^        | Bitwise XOR          | int result = a ^ b;   |
| ~        | Bitwise complement   | int result = ~a;      |
| <<       | Left shift           | int result = a << 2;  |
| \>>      | Right shift          | int result = a >> 2;  |
| \>>>     | Unsigned right shift | int result = a >>> 2; |

## Ternary Operator
| Operator | Description           | Example                    |
|----------|-----------------------|----------------------------|
| ?:       | Shorthand for if-else | int max = (a > b) ? a : b; |

## Instanceof Operator
| Operator   | Description       | Example                    |
|------------|-------------------|----------------------------|
| instanceof | Check object type | if (obj instanceof String) |

## Type Casting
| Operator | Description               | Example                   |
|----------|---------------------------|---------------------------|
| (type)   | Convert variable type     | double d = (double) a;    |

## String Concatenation
| Operator | Description  | Example                     |
|----------|--------------|-----------------------------|
| +        | Join strings | String s = "Hi " + "There"; |

## Precedence/Grouping
| Operator | Description              | Example                   |
|----------|--------------------------|---------------------------|
| ()       | Group expressions        | result = (a + b) * c;     |
| []       | Array element access     | int val = arr[2];         |
