### Complete and commit and push each task below. Parts of the code are shown as hints, the rest has been "redacted." 

1) Write a statement which logs 'Hi, my name is Chris and I'm 29 years old' to the console (use your name and you can lie about your age). 

> Notice the single quote in `... and I'm ...`

```
console.....('Hi, my name is....');
```

- Remember to commit and push

2) Wrap the statement in a function called `createGreeting` and call that function

```
function createGr.... {
  console.....('Hi, name is is........');
}

createGreeting();
```

- Remember to commit and ...

3) Have the function **return** the greeting instead of logging it out. Then invoke the function, capture the returned value, and log that out.

```
function createGreeting() {
  return ...
}

const greeting1 = createGreeting();
console.log(greeting1);
```

- Remember to commit and ...

4) Change the hardcoded string so it uses parameters passed into the function: `name` and `age`

```
function createGreeting(name, age){ 
  return ...
}
```

- Remember to ...

5) Create a variable named `yearOfBirth` and calculate the year based on age (ex. 2016 - age). Then add a sentence to the return value which outputs 'I was born in [yearOfBirth]'.

```
function createGreeting(name, age){ 
  const yearOf..........16 - age;
  return ...
}
```

- Just do it...

6) Move the year of birth calculation into a new function which returns the value expected. 

```
function getYearOfBirth(age){
  return ...
}

function createGreeting(name, age){
  const yob = .....
  return ...
}
```

- Is it a habit yet?

7) What happens if you enter a negative age? The function wouldn't cause an error but the result wouldn't make sense. Let's force an error if it's negative and add a `try/catch` when we call the top-level `createGreeting`...


```
function yearOfBirth(age){
  if () ...
    throw new Error("Age can not be negative");
	
  return ...;
}

.
.
.

try {
  const greeting1 = createGreeting(...);
} catch ...
```

- Commit, push.

7) Check if `name` and `age` have been entered. If not, create a conditional which throws an error with the message: 'Arguments not valid'.

> Hint: How do you check if a parameter or variable has not been "defined"?


8) What happens if you pass `"29"` (string) as the age? What about `"twenty nine"`? Implement a check to ensure the name is a `string` and the age is a `number`. If not, `throw new TypeError()`.

> Hint: `typeof age`
> Investigate: What is `NaN`?

---

Once completed, check your file against [this solution](solutions/function-drills-1-solution.md). This is for reference only once you've completed the task, NOT to help with the challenge. You should work through the exercise with your pair and consult a TA for help first.
