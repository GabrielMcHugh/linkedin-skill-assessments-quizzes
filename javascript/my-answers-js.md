###Q1. Which operator returns true if the two compared values are not equal?
My answer: !==
Correct

Note: ==! isnt anything

###Q2. How is a forEach statement different from a for statement?

My answer: A for statement is generic, but a forEach statement can be used only with an array.
Correct

###Q3. How would you use this function to find out how much tax should be paid on $50?

My answer: addTax(50)
Correct

###Q4. Which statement is the correct way to create a variable called rate and assign it the value 100?

My answer: let rate = 100
Correct

###Q5. Which statement creates a new Person object called "student"?

My answer: var student = new Person();
Correct

###Q6. When would the final statement in the code shown be logged to the console?

My answer: After 10 seconds
Incorrect

Why: setTimeout is changing the hidden property of modal. But console.log isn't within it and isn't waiting on it.

###Q7. When would 'results shown' be logged to the console?

Note: I don't this question is correct. I think the code for Q7 and Q6 have been mixed up. Or the code for this is wrong.

###Q8. You've written the code shown to log a set of consecutive values, but it instead results in the value 5, 5, 5, and 5 being logged to the console. Which revised version of the code would result in the value 1, 2, 3 and 4 being logged?

My answer:
```js
for (var i = 1; i <= 4; i++) {
  (function (j) {
    setTimeout(function () {
      console.log(j);
    }, j * 1000);
  })(i);
}
```
Correct

Why: function (j) is anonymouse and i is passed in as the parameter. So code no longer logs i which has already incremented to 5. Instead a new function is ran every increment with that loops i value being passed into j and logged.

###Q9. How does a function create a closure?

My answer: It returns a reference to a variable in its parent scope.
Correct

Why: Other functions can't access this variable. As theyre not within it's scope. Furthermore, the variable is initialised only once by the anonymouse function. Now nothing can access it except through the returned function.

###Q10. Which statement creates a new function called discountPrice?

My answer:
```js
let discountPrice = function (price) {
  return price * 0.85;
};
```
Correct


