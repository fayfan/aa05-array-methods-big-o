# Array practice

Identify the time complexity of each of these functions with a 1 sentence
justification for your answer. Assume `arr` is an array of length _n_.

## `arr.push()`

Time complexity: O(1)
Space complexity: O(1)
Justification: This function only requires adding an element to the length + 1 index of an array, so it is not affected by the length of the array, meaning that this function has constant time & space complexities

[push on MDN][push]

## `arr.pop()`

Time complexity: O(1)
Space complexity: O(1)
Justification: This function only requires removing an element from the length - 1 index of an array, so it is not affected by the length of the array, meaning that this function has constant time & space complexities

[pop on MDN][pop]

## `arr.shift()`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function requires taking every element of an array & decreasing its index by 1 so that the element at the start of the array can be removed, so it is affected by the length of the array, meaning that this function has linear time & space complexities

[shift on MDN][shift]

## `arr.unshift()`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function requires taking every element of an array & increasing its index by 1 so that a new element can be added to the start of the array, so it is affected by the length of the array, meaning that this function has linear time & space complexities

[unshift on MDN][unshift]

## `arr.splice()`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function removes &/or inserts elements at any position in an array; worst case scenario, it will remove/add an element at index 0, functioning similarly to `arr.shift()`/`arr.unshift()` as described above & giving it similar time & space complexities

[splice on MDN][splice]

## `arr.slice()`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function returns a copy of an array from indices n to length - 1 (if a 2nd index is not provided), meaning that the entire array from indices 0 to length - 1 may be returned in the worst case scenario, giving this function linear time & space complexities

[slice on MDN][slice]

## `arr.indexOf()`

Time complexity: O(n)
Space complexity: O(1)
Justification: The only way to find the index of 'n' is by going through the array starting from the first element until it finds an element with the value 'n', meaning that this function may take up to 'n' iterations &, therefore, has a linear time complexity; this function only requires storing 'n', so it has a constant space complexity

[indexOf on MDN][indexOf]

## `arr.map()`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function creates a new array by calling a callback function on every element of the array, so it is affected by the length of the array, meaning that this function has linear time & space complexities

[map on MDN][map]

## `arr.filter()`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function creates a new array with all elements of the array that pass the given test, so it is affected by the length of the array, meaning that this function has linear time & space complexities

[filter on MDN][filter]

## `arr.reduce()`

Time complexity: O(n)
Space complexity: O(1)
Justification: This function iterates through every element of the array but returns only a single value, so only its time complexity is affected by the length of the array, meaning that this function has a linear time complexity & a constant space complexity

[reduce on MDN][reduce]

## `arr.reverse()`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function creates a copy of the array with its elements in reverse order by iterating through each element of the array, so it is affected by the length of the array, meaning that this function has linear time & space complexities

[reverse on MDN][reverse]

## `[...arr]`

Time complexity: O(n)
Space complexity: O(n)
Justification: This function iterates through each element of an array to allow them to be called one-by-one, so it is affected by the length of the array, meaning that this function has linear time & space complexities

[spread on MDN][spread]

[push]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push
[pop]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop
[shift]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift
[unshift]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/unshift
[splice]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice
[slice]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice
[indexOf]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf
[map]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
[filter]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter
[reduce]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce
[reverse]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse
[spread]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax
