Complete the solution so that the function will break up camel casing, using a space between words.

```
function solution(string) {
    return string.replace(/([A-Z])/g, " $1")
}

solution('camelCasing')
solution('camelCasingTest')
```
