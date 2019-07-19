# CodewarsSolutions
### 1. Sum of positive - 8 kyu
[https://www.codewars.com/kata/5715eaedb436cf5606000381]
* 
```javaScript
 function positiveSum(arr){
   let sum = 0;
   for (let i = 0; i < arr.length; i++) {
     if (arr[i] >= 0) 
      sum =sum + arr[i];
   }
   return sum;
 }
``` 
*
```javaScript
 function positiveSum(arr) {
   return arr.reduce((accum, current) => accum + (current > 0 ? current : 0), 0);
 }
```
*
```javaScript
 function positiveSum(arr) {
   return arr.filter(el => el > 0).reduce((a, c) => a + c, 0);
 }
``` 
 
### 2. Calculate average
 [https://www.codewars.com/kata/calculate-average/train/javascript]
```javaScript
const find_average = array => array.reduce((accum, current) => accum + current,0) / array.length;
```  
### 3.  Maximum Triplet Sum (Array Series #7)
[https://www.codewars.com/kata/maximum-triplet-sum-array-series-number-7/train/javascript]
* 
```javaScript
 function maxTriSum(numbers){
   let sum = 0;
     let res = numbers.sort((a, b) => b - a);
     let arr = [];
     for (let i = 0; i < res.length; i++){
       if (arr.length >= 3){
         break
       }
         if (!arr.includes(res[i])){
           arr.push(res[i]);
           sum += res[i];
         }
     }
     return sum;
 }
```
* 
```javaScript
function maxTriSum(numbers){
  return numbers.filter((el, i )=> i === numbers
                .lastIndexOf(el))
                .sort((a, b) => a - b)
                .slice(-3)
                .reduce((a, b) => a + b, 0);
}
``` 
*
```javaScript
function maxTriSum(numbers){
  let set = new Set(numbers);
    set = [...set].sort((a, b) => b - a);
      return set[0] + set[1] + set[2];
}
```
 ### 4. Array plus array - 8 kyu
 [https://www.codewars.com/kata/array-plus-array/train/javascript]
 *
 ```javaScript
 function arrayPlusArray(arr1, arr2) {
   let sum = 0;
     for (let i = 0; i < arr1.length; i++){
       sum += arr1[i];
       }
       for(let i = 0; i < arr2.length; i++){
         sum += arr2[i];
         }
   return sum; 
 }
 ```
 *
 ```javaScript
 function arrayPlusArray() {
   let res = 0;
     for (let i = 0 ; i < arguments.length; i += 1) {
 
       for (let j = 0; j < arguments[i].length ; j += 1) {
 
         res += arguments[i][j];
       }
     }
    return res;
 }
```
*
```javaScript
function arrayPlusArray(arr1, arr2) {
  return arr1.concat(arr2).reduce((acc, cur) => acc + cur);
}
```
*
```javaScript
const arrayPlusArray = (arr1, arr2) =>
  [...arr1, ...arr2].reduce((total, value) => total + value, 0);
  ```
### 5. Count Odd Numbers below n - 8 kyu
[https://www.codewars.com/kata/count-odd-numbers-below-n/train/javascript]
*
```javaScript
function oddCount(n) {
  return Math.floor(n/2);
}
```
### 6. Multiples of 3 or 5 - 6 kyu
[https://www.codewars.com/kata/multiples-of-3-or-5/train/javascript]
*
```javaScript
function solution(number){
  let sum = 0; 
    for (let i = 3; i < number; i++){
      if(i % 3 === 0 || i % 5 === 0){
        sum += i;
      }
    }
    return sum;
}
```
### 7. Loading Kata: Sum Mixed Array - 8 kyu
[https://www.codewars.com/kata/sum-mixed-array/train/javascript]
*
```javaScript
function sumMix(x){
  let sum = 0;
    for (let i = 0; i < x.length; i++){
      if (typeof x[i] === 'string'){
        x[i] = Number(x[i])
      }
      sum += x[i]; 
    }
   return sum; 
} 
```
*
```javaScript
const sumMix = x => x.reduce((total, value) => total + Number(value), 0);
```
### 8. Who is going to pay for the wall? - 8 kyu
[https://www.codewars.com/kata/58bf9bd943fadb2a980000a7/solutions/javascript/me/best_practice]
*
```
function whoIsPaying(name){
  let array = [name];
    if(name.length > 2){
      let str = name.substring(0, 2);
      array.push(str); 
    }
   return array; 
}
```
### 9. 
[]
*
```javaScript


```
