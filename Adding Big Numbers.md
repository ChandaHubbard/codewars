#### We need to sum big numbers and we require your help.

#### Write a function that returns the sum of two numbers. The input numbers are strings and the function must return a string.

- Example

  `add("123", "321")` -> `444`
  
  `add("11", "99")`   -> `110`

- Notes

  - The input numbers are big.
  - The input is a string of only digits
  - The numbers are positives

#

```
function add(a, b) {
  return BigInt(Math.ceil((Number(a) + Number(b)))).toString(); 
}

add("123", "321")
add("11", "99")
add("1", "1")
add("123", "456")
add("888", "222")
add("1372", "69")
add("12", "456")
add("101", "100")
add("63829983432984289347293874", "90938498237058927340892374089")
```
