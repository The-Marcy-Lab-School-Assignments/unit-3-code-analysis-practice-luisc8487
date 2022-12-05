# unit-3-code-analysis-practice

Using markdown, identify what the following code block does and explain how the `forEach` function works.

```js
function forEach(arr, action) {
  for (let i = 0; i < arr.length; i++) {
    action(arr[i]);
  }
}

forEach(['a', 'b', 'c'], console.log);
```

**Guiding Questions:**
* What does the code do (what does it print? are any variable reassigned? etc...)
* What are the expected data types for each of the parameters?
* When the function is invoked, what value are provided as arguments?
* How does `forEach` use the provided arguments?

**Key Terms to use**: parameters, arguments, invoke/invocation, iterate, "element of the array", increment,  

<hr>

Your explanation here...

The code above logs `"a"` `"b"` `"c"`. In `function forEach`, `arr` and `action` has been set as parameters. The for loop iterates through the `arr` where we can access each element in the `arr`. Next line states `action` will accpet an argument of `arr[i]`. `arr[i] = a b or c` depending on iteration value. So when `forEach()` is invoked with two parameters being `["a", "b", "c"]` and `console.log` we are actually passing that value of `["a", "b" "c"]` to `arr` and `console.log` to `action`. So when `action(arr[i])` gets executed, we are passing this `console.log(arr[i])` hence why we get `"a" "b" "c"`