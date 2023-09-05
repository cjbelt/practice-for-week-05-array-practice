# Array practice

Identify the time complexity of each of these functions with a 1 sentence
justification for your answer. Assume `arr` is an array of length _n_.

## `arr.push()`

Time complexity: O(1)
Space complexity: O(1)
Justification: The amount of operations needed in this method to add a element in the array is only one, as well as the amount of data storing.

[push on MDN][push]


## `arr.pop()`

Time complexity: O(1)
Space complexity: O(1)
Justification: the arr.pop() method just removes the last element of the array, making the same amount of operations and storing the same amount of data.

[pop on MDN][pop]

## `arr.shift()`

Time complexity: O(n)
Space complexity: O(1)
Justification: Like in the arr.pop() method, arr.shift() removes an element from the array, in this case the first of it. But it have to rearrange all its remaining elements increasing the number of operations linearly according to the length of the array. There's no need to store new data on this process, therefore the space complexity is constant.

[shift on MDN][shift]

## `arr.unshift()`

Time complexity: O(n)
Space complexity: O(1)
Justification: like in the push method, arr.shift adds new elements in the array, in this case, in the beggining of it. The method needs to rearrange all the array's one index forward to include the new element, defining the number of operations according to the length of the array. The method just adds one new element to the array, therefore it have a constant space complexity.

[unshift on MDN][unshift]

## `arr.splice()`

Time complexity: O(n)
Space complexity: O(n)
Justification: this method creates a new array based in a existing one, excluding some elements and adding new ones, and then replacing the original array with the new array. The time and space complexity of the method mainly depends on the length of the array, increasing the complexity linearly.

[splice on MDN][splice]

## `arr.slice()`

Time complexity: O(n)
Space complexity: O(n)
Justification: the slice method creates a new array based on an existing array. The complexity of the method depends mainly on the length of the array, increasing it linearly.

[slice on MDN][slice]

## `arr.indexOf()`

Time complexity: O(n)
Space complexity: O(1)
Justification: the indexOf method will seek for an array's element that matches the giving argument. The time complexity grows, on average, linearly, depending on the length of the array and the position of the element. The only new data that needs to be stored is the argument, therefore the space complexity is constant.

[indexOf on MDN][indexOf]

## `arr.map()`

Time complexity: O(n)
Space complexity: O(n)
Justification: since the map method iterates over each element of the array to call a function, the time complexity will grow linearly depending on the length of the array, and since a new element will be added to a new array for each function call, the space complexity is also linear, depending on the length of the array.

[map on MDN][map]

## `arr.filter()`

Time complexity: O(n)
Space complexity: O(n)
Justification: the arr.filter method iterates over each element of the array calling a function. Therefore, the time complexity will increase linearly depending on the length of the array. The space complexity will depends on the amount of elements that satisfies the function's condition, so it will increase linearly relative to them.

[filter on MDN][filter]

## `arr.reduce()`

Time complexity: O(n)
Space complexity: O(1)
Justification: arr.reduce iterates over each element of the array calling a function, increasing the time complexity linearly relative to the length of the array. The space complexity is constant because the only new data to be stored is the function of the argument (if it wasn't declared before) and the accumulator and the current element variables.

[reduce on MDN][reduce]

## `arr.reverse()`

Time complexity: O(n)
Space complexity: O(1)
Justification: the time complexity depends on the length of the array, as the method will iterate through the elements of the array to switch the elements positions. The space complexity is constant because the only new data will be the variables required to switch two elements positions that will be reused in each iteration,as the reversing happens in place.

[reverse on MDN][reverse]

## `[...arr]`

Time complexity: O(n)
Space complexity: O(n)
Justification: the spread operator will iterate over each element of the array to spread it, therefore the time complexity is linear. The space complexity is also linear when the spread operator is inside an array because the program will create a deep copy of the original array.

[spread on MDN][spread]

[push]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push
[pop]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop
[shift]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift
[unshift]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift
[splice]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice
[slice]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice
[indexOf]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf
[map]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
[filter]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter
[reduce]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce
[reverse]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse
[spread]:https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax
