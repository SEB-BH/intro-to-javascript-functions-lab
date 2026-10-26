<h1>
  <span class="headline">Intro to JavaScript Functions Lab</span>
  <span class="subhead">Exercise</span>
</h1>
## Instructions

In these exercises, you will practice writing functions using the JavaScript concepts you've learned so far.

You will use:

- Variables and data types
- Operators and comparisons
- `if`, `else if`, and `else` statements
- Parameters and arguments
- The `return` keyword

For each exercise:

1. Create a function with the name provided.
2. Add the required parameters.
3. Write the code inside the function.
4. Use `return` to send the result back.
5. Run your JavaScript file with Node.js to test your function.

The first exercise has been completed for you as an example.

> 💡 **Remember:** Your functions should `return` the answer, not `console.log()` it. We've already provided `console.log()` statements to help you test your work.

---

### Exercise 1: `generateEmail()`

**This exercise has been completed for you.**

Imagine you're building a system that creates email addresses for new employees.

Create a function called `generateEmail()` that:

1. Accepts two parameters: `username` and `domain`.
2. Combines them into an email address with an `@` symbol between them.
3. Returns the completed email address as a string.

```js
function generateEmail(username, domain) {
  return `${username}@${domain}`
}

// Test the function
console.log('Exercise 1 Result:', generateEmail("sara", "company.com")) // sara@company.com
console.log('Exercise 1 Result:', generateEmail("ali", "example.com")) // ali@example.com
console.log('Exercise 1 Result:', generateEmail("fatima", "school.edu")) // fatima@school.edu
```

**Try it:** Change the arguments in one of the function calls to create a different email address.

Notice how the function works with different usernames and domains without changing the code inside the function.

---

### Exercise 2: `greetUser()`

Imagine you're building a website that welcomes users when they sign in.

Create a function called `greetUser()` that:

1. Accepts two parameters: `name` and `timeOfDay`.
2. Uses those parameters to create a greeting.
3. Returns the greeting as a string.

The `timeOfDay` argument will be `"morning"`, `"afternoon"`, or `"evening"`.

> 💡 **Hint:** You don't need an `if` statement for this exercise. Think about how you can use a template literal to create the greeting.

**Example:** `greetUser("Sara", "morning")` should return `"Good morning, Sara!"`.

```js
// Write your function here



// Test your function
console.log('Exercise 2 Result:', greetUser("Sara", "morning")) // Good morning, Sara!
console.log('Exercise 2 Result:', greetUser("Ali", "afternoon")) // Good afternoon, Ali!
console.log('Exercise 2 Result:', greetUser("Fatima", "evening")) // Good evening, Fatima!
```

---

### Exercise 3: `calculateVAT()`

In Bahrain, the standard Value Added Tax (VAT) rate is 10%.

Create a function called `calculateVAT()` that:

1. Accepts two parameters: `price` and `vatPercentage`.
2. Calculates the VAT amount using the provided percentage.
3. Returns the VAT amount, **not the total price**.

For example, if an item costs 50 BHD and the VAT rate is 10%, the VAT amount is 5 BHD.

> 💡 **Hint:** To calculate a percentage, divide it by 100. For example, 10% of 50 is `50 * (10 / 100)`.

```js
// Write your function here



// Test your function
console.log('Exercise 3 Result:', calculateVAT(50, 10)) // 5
console.log('Exercise 3 Result:', calculateVAT(100, 10)) // 10
console.log('Exercise 3 Result:', calculateVAT(200, 5)) // 10
```

---

### Exercise 4: `checkStock()`

Imagine you're building an online store. Before customers place an order, you need to check whether a product is available.

Create a function called `checkStock()` that:

1. Accepts one parameter: `quantity`.
2. Uses an `if...else` statement to check the quantity.
3. Returns the string `"In stock"` if the quantity is greater than 0.
4. Returns the string `"Out of stock"` if the quantity is 0.

> 💡 **Hint:** You can use the greater than operator (`>`) to check whether there are any items available.

```js
// Write your function here



// Test your function
console.log('Exercise 4 Result:', checkStock(10)) // In stock
console.log('Exercise 4 Result:', checkStock(0))  // Out of stock
console.log('Exercise 4 Result:', checkStock(1))  // In stock
```
---

### Exercise 5: `maxOfTwoNumbers()`

Create a function called `maxOfTwoNumbers()` that:

1. Accepts two parameters: `numA` and `numB`.
2. Uses an `if...else` statement to compare the two numbers.
3. Returns the larger number.
4. If both numbers are equal, returns that number.

> 💡 **Hint:** You can use `>=` to compare the two numbers. Remember that `return` immediately stops the function.

```js
// Write your function here



// Test your function
console.log('Exercise 5 Result:', maxOfTwoNumbers(3, 9)) // 9
console.log('Exercise 5 Result:', maxOfTwoNumbers(15, 4)) // 15
console.log('Exercise 5 Result:', maxOfTwoNumbers(7, 7)) // 7
```

---

### Exercise 6: `isCharAVowel()`

A **vowel** is one of these letters: `a`, `e`, `i`, `o`, or `u`.

Create a function called `isCharAVowel()` that:

1. Accepts one parameter: `char`.
2. Checks whether `char` is a vowel.
3. Returns the boolean `true` if it is a vowel.
4. Returns the boolean `false` if it is not a vowel.

For this exercise, you can assume all letters are lowercase. The letter `y` is not considered a vowel.

> 💡 **Hint:** You can use the strict equality operator (`===`) and the OR operator (`||`) to check multiple conditions.

```js
// Write your function here



// Test your function
console.log('Exercise 6 Result:', isCharAVowel("a")) // true
console.log('Exercise 6 Result:', isCharAVowel("e")) // true
console.log('Exercise 6 Result:', isCharAVowel("b")) // false
console.log('Exercise 6 Result:', isCharAVowel("y")) // false
```

---

### Exercise 7: `maxOfThree()`

In Exercise 5, you wrote a function that compared two numbers. Now let's try comparing three!

Create a function called `maxOfThree()` that:

1. Accepts three parameters: `numA`, `numB`, and `numC`.
2. Uses conditional statements to compare the three numbers.
3. Returns the largest number.

If two or more numbers are equal and are the largest, return that number.

> 💡 **Hint:** You can use `if`, `else if`, and `else` statements. You can also use the AND operator (`&&`) to check whether a number is greater than or equal to both other numbers.

```js
// Write your function here



// Test your function
console.log('Exercise 7 Result:', maxOfThree(5, 10, 8)) // 10
console.log('Exercise 7 Result:', maxOfThree(20, 5, 10)) // 20
console.log('Exercise 7 Result:', maxOfThree(3, 7, 15)) // 15
console.log('Exercise 7 Result:', maxOfThree(8, 8, 4)) // 8
```

---

### Exercise 8: `convertTemperature()`

Create a function called `convertTemperature()` that converts temperatures between Celsius and Fahrenheit.

Your function should:

1. Accept two parameters: `temperature` and `scale`.
2. If `scale` is `"C"`, convert the temperature from Celsius to Fahrenheit.
3. If `scale` is `"F"`, convert the temperature from Fahrenheit to Celsius.
4. Return the converted temperature as a number.

For this exercise, you can assume `scale` will always be either `"C"` or `"F"`.

**Use these formulas:**

Celsius to Fahrenheit:

```js
(temperature * 9 / 5) + 32
```

Fahrenheit to Celsius:

```js
(temperature - 32) * 5 / 9
```

> 💡 **Hint:** Use an `if...else` statement to decide which formula to use.

```js
// Write your function here



// Test your function
console.log('Exercise 8 Result:', convertTemperature(0, "C")) // 32
console.log('Exercise 8 Result:', convertTemperature(32, "C")) // 89.6
console.log('Exercise 8 Result:', convertTemperature(32, "F")) // 0
console.log('Exercise 8 Result:', convertTemperature(212, "F")) // 100
```

---

### Exercise 9: `basicCalculator()`

For your final exercise, you'll create a simple calculator that can perform four different operations.

Create a function called `basicCalculator()` that:

1. Accepts three parameters: `numA`, `numB`, and `operation`.
2. Checks the value of `operation` using conditional statements.
3. Performs the correct calculation.
4. Returns the result.

The `operation` parameter will be one of these strings:

- `"add"` — Add the two numbers.
- `"subtract"` — Subtract `numB` from `numA`.
- `"multiply"` — Multiply the two numbers.
- `"divide"` — Divide `numA` by `numB`.

For this exercise, you can assume that the operation will always be valid and that you will not divide by zero.

> 💡 **Hint:** Use `if`, `else if`, and `else` statements to check the operation. Remember that you can return the result directly from each condition.

```js
// Write your function here



// Test your function
console.log('Exercise 9 Result:', basicCalculator(10, 5, "add")) // 15
console.log('Exercise 9 Result:', basicCalculator(10, 5, "subtract")) // 5
console.log('Exercise 9 Result:', basicCalculator(10, 5, "multiply")) // 50
console.log('Exercise 9 Result:', basicCalculator(10, 5, "divide")) // 2
```


🎉  You did it!  🎉
