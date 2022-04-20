# useReducer-

for self understanding
`const numbers = [2, 4, 6];

const sum = numbers.reduce(function summarize(sum, number) {
	console.log(`before: sum= ${sum} , number =${number}`)                            // 0  2, 2 4, 6 6
  const updatedSum = sum + number;                                                  // 2 , 6, 12
console.log(`After: sum= ${sum} , number =${number}, updateSum=${updatedSum}`)      //  0 2 2,  2 4 6,   6 6 12
  return updatedSum;                                                                //2, 6, 12
}, 0);

console.log(sum);                                                                   // 12
`



> numbers.reduce(summarize, 0) calculates the sum of all elements in the array.

> The summarize callback is invoked for every item in the array with the accumulated sum and the iterated number. summarize callback adds the iterated item to the already accumulated sum, and returns that updated sum.

> That's how an array is reducing to a sum.

> Also, note the second argument of numbers.reduce(summarize, 0) — the sum of array items is initialized with 0.

Practice exc for useReducer

- [x] Find Even and Odd sum
- [x] Find Even and Odd sum without %2 logic

