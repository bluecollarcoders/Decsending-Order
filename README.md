# Decsending-Order

## Problem

Description:
Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

Examples:
Input: 42145 Output: 54421

Input: 145263 Output: 654321

Input: 123456789 Output: 987654321

## Solution

```javascript
const descendingOrder = (n) => {
//   convert number toSring()
  var convert = n.toString();
  
//   split parameter
  var newNum = convert.split('');

//   sort reverse
var reverse = newNum.sort((a,b) => b-a);
;
//   convert string back into number
return Number(reverse.join(''));
}

```
