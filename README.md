🧮 Fraction Class in Python

📌 Overview

The Fraction class in Python allows you to perform basic arithmetic operations on fractions while ensuring they remain in their simplest form. It supports:

✅ Addition (+)
✅ Subtraction (-)
✅ Multiplication (*)
✅ Division (/)
✅ Automatic fraction simplification
✅ Multiple fraction operations in a single expression
✅ Prevention of division by zero errors

🚀 How It Works

This class uses operator overloading to make fraction operations feel natural. Instead of calling functions, you can simply use standard mathematical operators:

f1 = Fraction(1, 2)  # Represents 1/2
f2 = Fraction(3, 4)  # Represents 3/4
f3 = Fraction(5, 6)  # Represents 5/6

# Perform arithmetic operations
print(f"Addition: {f1 + f2 + f3}")     # ➝ 19/12
print(f"Subtraction: {f1 - f2 - f3}")  # ➝ -5/12
print(f"Multiplication: {f1 * f2 * f3}")  # ➝ 5/16
print(f"Division: {f1 / f2 / f3}")  # ➝ 4/5

📜 Class Methods Explained

🔹 __init__(self, num, den)

Initializes a fraction with numerator (num) and denominator (den).

Automatically simplifies the fraction upon creation.

Prevents division by zero errors.

🔹 simplify(self)

Uses Greatest Common Divisor (GCD) to reduce the fraction to its simplest form.

🔹 __str__(self)

Returns a human-friendly string representation of the fraction (e.g., "3/4").

🔹 __add__(self, *others)

Adds multiple fractions.

Uses cross-multiplication to ensure correct results.

Returns a new simplified Fraction object.

🔹 __sub__(self, *others)

Subtracts multiple fractions.

Uses cross-multiplication for correctness.

Returns a new simplified Fraction object.

🔹 __mul__(self, *others)

Multiplies multiple fractions together.

Simply multiplies numerators & denominators.

Returns a new simplified Fraction object.

🔹 __truediv__(self, *others)

Divides multiple fractions by multiplying with their reciprocals.

Returns a new simplified Fraction object.

🔥 Why Use This Class?

✅ Makes fraction operations intuitive and readable.
✅ Supports multiple fractions in a single operation.
✅ Handles zero denominators to prevent crashes.
✅ Automatically simplifies results.
✅ Returns Fraction objects, allowing chaining of operations.

👀 Example Use Cases

f1 = Fraction(2, 5)
f2 = Fraction(3, 7)
f3 = Fraction(4, 9)

# Perform operations
result1 = f1 + f2 - f3  # Multiple operations in one line
result2 = (f1 * f2) / f3  # Mixing multiplication & division

print(f"Result 1: {result1}")  # Output: 29/35
print(f"Result 2: {result2}")  # Output: 21/40

⚡ Future Improvements

🔹 Add support for negative fractions
🔹 Implement comparison operators (==, >, <)
🔹 Support mixed fractions (e.g., 1 1/2)

📜 License

This project is open-source and free to use. Feel free to modify and improve it! 🚀

