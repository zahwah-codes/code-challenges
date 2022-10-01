ATM machines allow 4 or 6 digit PIN codes and PIN codes cannot contain anything but exactly 4 digits or exactly 6 digits.

If the function is passed a valid PIN string, return true, else return false.


### Thinking

- My first thought was to use a ternary operator to reduce the amount of code I would have to write using an if statement
- I decided to use the match() method to recieve the result of matching a string against a RegEx
- To match numbers 0 - 9, I used the expression /^[0-9]*$/g. I used *$ in order to match integers only. The ^ symbol matches anything that is between the brackets
- Since ATM machines only arrow 4 or 6 digits, I included the && operator to make sure that the pin.length is either 4 or 6


### Solution

```js

function validatePIN (pin) {

  return pin.match(/^[0-9]*$/g) && (pin.length === 4 || pin.length === 6) ? true : false
}

```