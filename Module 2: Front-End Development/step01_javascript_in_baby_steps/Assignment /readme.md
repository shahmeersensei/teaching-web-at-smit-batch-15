# 🔹 **1. Variables Practice Questions**
### (Understanding variable declaration, scope, and usage)

1. **User Input Storage:** Write a program that asks the user for their name and stores it in a variable. Then, print `"Hello, [name]!"`.
2. **Bank Balance Update:** Declare a variable `bankBalance` and assign it a value of `1000`. Deduct `200` when a user makes a withdrawal.
3. **Temperature Conversion:** Store a temperature in Celsius in a variable and convert it to Fahrenheit using the formula:  
   **`F = (C × 9/5) + 32`**
4. **Shopping Cart Total:** Declare a variable `cartTotal`, add the price of two items, and store the total.
5. **User Login Status:** Declare a variable `isLoggedIn` and assign it `true` if the user is logged in, otherwise `false`. Print the value.
6. **Variable Scope Test:** Declare a variable inside a function and try to access it outside the function. Explain what happens.
7. **Reassigning Variables:** Declare a variable using `let`, assign it a value, and then change it later in the code.
8. **Const vs Let:** Try to declare a variable with `const`, then attempt to change its value. Observe and explain the error.
9. **Using Template Literals:** Create a sentence using variables for a person's name and age:  
   `"My name is [name] and I am [age] years old."`
10. **Role-Based Access:** Create a variable `userRole` (values: "admin" or "user"). If the role is "admin," print `"Access granted"`, otherwise print `"Access denied"`.

---

# 🔹 **2. Operators Practice Questions**
### (Working with Arithmetic, Logical, and Comparison Operators)

1. **Simple Calculator:** Write a program that takes two numbers and prints their sum, difference, product, and quotient.
2. **Discount Calculation:** A shop gives a 10% discount on purchases above `500`. Write a program to calculate the final price.
3. **Odd or Even:** Check if a given number is odd or even using the modulus (`%`) operator.
4. **Voting Eligibility:** Check if a person is eligible to vote (age >= 18).
5. **Logical AND/OR Example:** A person can enter a movie if they are older than `12` or accompanied by an adult. Implement this using `&&` and `||` operators.
6. **Password Strength Checker:** A password is strong if it has at least 8 characters and contains a number. Check if a given password meets the criteria.
7. **Driving License Check:** A person can apply for a driving license if they are 18 or older and have passed the test. Use logical operators.
8. **Max of Three Numbers:** Write a program that takes three numbers and prints the largest one using comparison operators.
9. **Swapping Two Numbers Without a Third Variable:** Swap two numbers using arithmetic operations (`+` and `-`) instead of a temporary variable.
10. **Ternary Operator Usage:** Write a one-liner using the ternary operator that prints `"Adult"` if age >= 18 and `"Minor"` otherwise.

---

# 🔹 **3. Data Types Practice Questions**

### ✅ **(A) String Practice Questions**
1. **Reverse a String:** Take a user's name as input and print it in reverse order.
2. **Count Characters in a String:** Ask the user for a sentence and print how many characters it contains.
3. **Extract Initials from Name:** Given `"Amit Kumar"` → Print `"A.K."`
4. **Check Palindrome:** Write a function to check if a given word is the same forwards and backwards.
5. **Replace Words:** Replace `"bad"` with `"good"` in the sentence `"This is a bad day"` using JavaScript string methods.
6. **Convert Case:** Convert `"hello world"` to uppercase and `"HELLO WORLD"` to lowercase.
7. **Email Validator:** Check if an email contains `"@"` and `"."` in the correct order.
8. **Find Position of a Word:** Find the index of `"JavaScript"` in `"I love JavaScript programming."`
9. **Slice a String:** Extract `"coding"` from `"I enjoy coding every day"`.
10. **String Concatenation:** Combine two strings `"Hello"` and `"World"` using `+` and template literals.

---

### 🔢 **(B) Number Practice Questions**
1. **Find the Square and Cube:** Take a number and print its square and cube.
2. **Round a Number:** Round `7.49` to the nearest integer.
3. **Random Dice Roll:** Generate a random number between 1 and 6.
4. **Simple Interest Calculation:** Given principal, rate, and time, calculate the interest.
5. **Currency Converter:** Convert USD to INR (1 USD = 82 INR).
6. **Extract Decimal Part:** From `9.85`, extract and print `.85`.
7. **Find Remainder:** Find the remainder when `55` is divided by `6`.
8. **Temperature in Decimal:** Convert temperature and round it to 2 decimal places.
9. **Age Calculator:** Given the birth year, calculate the person’s age.
10. **Power of a Number:** Calculate `2^5` using JavaScript's `Math.pow()`.

---

### ✅ **(C) Boolean Practice Questions**
1. **Light Bulb Status:** A light bulb can be ON (true) or OFF (false). Toggle its state.
2. **Weather Check:** If the temperature is below 0°C, return `true` (cold), otherwise return `false`.
3. **Check for Empty Input:** If a user enters an empty string, return `false`.
4. **User Authentication:** If a username and password match, return `true`, else return `false`.
5. **Check Leap Year:** A year is a leap year if it's divisible by `4` but not by `100`, unless also divisible by `400`.
6. **Check Prime Number:** Return `true` if a number is prime, else return `false`.
7. **Two Numbers Equal:** Return `true` if two given numbers are equal.
8. **String Starts With:** Check if a string starts with `"Hello"`.
9. **Voting Eligibility (Boolean Return):** Return `true` if age is 18 or above.
10. **Boolean Flip:** Write a function that takes a boolean value and returns the opposite (`true` → `false`, `false` → `true`).

---

### 🔹 **(D) Array Practice Questions**
1. **Find Maximum in Array:** Given `[10, 20, 5, 30]`, find the largest number.
2. **Find Sum of All Elements:** Given `[2, 4, 6, 8]`, find the total sum.
3. **Reverse an Array:** Reverse the order of elements in `[1, 2, 3, 4, 5]`.
4. **Remove Duplicates:** Remove duplicate values from `[1, 2, 2, 3, 4, 4, 5]`.
5. **Find Even Numbers:** Filter out only even numbers from `[5, 10, 15, 20, 25]`.
6. **Join Elements:** Convert `["Apple", "Banana", "Cherry"]` into `"Apple-Banana-Cherry"`.
7. **Check if Exists:** Check if `"Banana"` exists in an array.
8. **Sort an Array:** Sort `[5, 2, 9, 1, 3]` in ascending order.
9. **Find Index of Element:** Find the position of `30` in `[10, 20, 30, 40]`.
10. **Slice an Array:** Extract the first three elements from `[100, 200, 300, 400, 500]`.

---

### 🔹 **(E) Object Practice Questions**
1. **Create a Student Object:** Store name, age, and marks.
2. **Retrieve a Property:** Get the `"name"` value from `{name: "Rahul", age: 20}`.
3. **Modify an Object:** Change a student's marks from `85` to `90`.
4. **Check Property Exists:** Check if `"age"` exists in `{name: "Amit"}`.
5. **Loop Through an Object:** Print all key-value pairs in an object.
6. **Nested Objects:** Create an object representing a laptop with specifications.
7. **Object Length:** Find the number of properties in `{a:1, b:2, c:3}`.
8. **Delete a Property:** Remove `"age"` from an object.
9. **Merge Two Objects:** Combine `{a:1}` and `{b:2}`.
10. **Convert Object to Array:** Convert `{a:10, b:20}` into `[['a', 10], ['b', 20]]`.
