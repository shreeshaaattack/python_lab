PROBLEM STATEMENT :
Demonstrate various Data Types and Operators in Python.

ALGORITHM:
STEP 1 : Start the program.
STEP 2 : Declare two integer variables x and y and assign them numeric values.
STEP 3 : Display results of arithmetic expressions using addition, subtraction, multiplication, and power operators.
STEP 4 : Use comparison operators to check mathematical identities and print whether they are true or false.
STEP 5 : Perform bitwise operations such as AND (&), OR (|), and XOR (^) on the variables.
STEP 6 : Demonstrate how addition and subtraction can also be represented using bitwise operators.
STEP 7 : Print the results of all expressions using the print() function.
STEP 8 : Stop the program.

SOURCE CODE:
x=int(input("Enter the value for x:"));
y=int(input("Enter the value for y:")); 

print("\nEquation Assignment Operators:")
print((x + y) ** 2 == x**2 + 2*x*y + y**2)
print((x - y) ** 2 == x**2 - 2*x*y + y**2)
print((x + y) * (x - y) == x**2 - y**2)
print(x**3 + y**3 == (x + y) * (x**2 - x*y + y**2))

print("\nBitwise Operator Demonstration:")
print(x | y == (x ^ y) + (x & y))
print(x ^ (x & y) == (x | y) ^ y)
print(y ^ (x & y) == (x | y) ^ x)
print((x & y) ^ (x | y) == x ^ y)

print("\nAddition using Bitwise Operators:")
print(x + y == (x | y) + (x & y))
print(x + y == (x ^ y) + 2*(x & y))

print("\nSubtraction using Bitwise Operators:")
print(x - y == (x ^ (x & y)) - ((x | y) ^ x))
print(x - y == ((x | y) ^ y) - ((x | y) ^ x))
print(x - y == (x ^ (x & y)) - (y ^ (x & y)))
print(x - y == ((x | y) ^ y) - (y ^ (x & y)))

OUTPUT:
Enter the value for x:78
Enter the value for y:908

Equation Assignment Operators:
True
True
True
True

Bitwise Operator Demonstration:
True
True
True
True

Addition using Bitwise Operators:
True
True

Subtraction using Bitwise Operators:
True
True
True
True

=== Code Execution Successful ===
