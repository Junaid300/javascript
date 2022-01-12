## Short Cirtuiting in Javascript
### Operators List
1. OR Operator ( || )
2. AND Operator ( && )
3. Nullish Coalescing ( ?? )

### OR OPERATOR ( || )
`true || false`
##### As we know In OR operator, if it will find any true value. It will return true otherwise return false.
##### Let have a look on this example
`true || false`
##### what will be result? Definitly true.
`0 || 'Hello World'` 
##### Now what will be answer of this example ? As 0 is behaved as false. And Hello World is behaved as True. Answer is True. Right?
##### NO. || return true value not boolean value.  In this case Answer is `Hello World`
##### If it finds truthy value return truthy value other wise return last value.
`'' || 'Junaid'`
##### `'' || 'Junaid'` , it will return truthy value that is Junaid.
##### `true || 0`, it will return true.
 `undefined || null`
 #####  `undefined || null` . Now what with this example ? Both are fasly value now what will it return ?
 ##### If it finds truthy value return truthy value other wise return last value. So , Answer will be null here.
 
 `undefined || 0 || '' || 'Hello' || 23 || null`
 ##### Solve it yourself :D
 
 ### use Case
 ```
 let myAge;
 let age = myAge || 23
 // it will check myAge. if it is truthy then will return that value otherwise it will assign 23.
 //age = 23
 // In some case, we can use OR operator or Short circuiting instead of ternary operator.
 // age = myAge ? myAge : 23
 ```

 
