Trolls are attacking your comment section!

A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.

Your task is to write a function that takes a string and return a new string with all vowels removed.

For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".

> Note: for this kata y isn't considered a vowel.

### Thinking

- Using the javascript string replace() method to return a new string with the value(s) replaced.
- I thought of using the method RegEx as you're able to replace patterns and not just exact characters.
- I used [aeiou] as the first argument. The 'g' is the global flag which tells the function to look for a match over the entire string. The 'i' flag tells it to match case sensitivity (to match over *aeiou* and *AEIOU*).
- For the second argument, I kept it empty in order to remove all the vowels.

### Solution

```js

function disemvowel (str) {

  return str.replace(/[aeiou]/gi, '');

}

```