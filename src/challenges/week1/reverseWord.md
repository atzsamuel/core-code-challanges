# Reversed Words

`Example 1`

```
    "The greatest victory is that which requires no battle" --> "battle no requires which that is victory greatest The"
```
`My solution`

```js
function reverseWords(str){
        let result = "";
        let words = str.split(" ");
        for(let i = words.length - 1; i >= 0; i--) {
            result += words[i] + " ";
        }
        return result.trim();
   // reverse those words
}
```

`Others Solutions`
`Solution 1`

```js
function reverseWords(str){
  var reverse = [];
  var words = str.split(" ");
  for(let i=words.length-1; i>=0; i--){
    reverse.push(words[i]);
    
  }
  return reverse.join(" ")
}
```

`Solution 2`

```js
function reverseWords(str){
  return str.split(' ').reverse().join(' ');
}
```
