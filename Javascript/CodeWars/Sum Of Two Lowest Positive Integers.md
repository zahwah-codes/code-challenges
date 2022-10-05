Create a function that returns the sum of the two lowest positive numbers given an array of minimum 4 positive integers. No floats or non-positive integers will be passed.

For example, when an array is passed like [19, 5, 42, 2, 77], the output should be 7.

[10, 343445353, 3453445, 3453545353453] should return 3453455.


### Thinking

- My first thought was to use Math.min. However, I realised there is a much easier way which is using the sort() method. The sort method sorts the array from smallest to biggest number. I saved that into a variable which I returned afterwards using the indexes of 0 and 1.

### Solution

```js

function sumTwoSmallestNumbers(numbers) {

  const ordered = numbers.sort(function(a,b){return a-b;});

  return ordered[0] + ordered[1]

}

```