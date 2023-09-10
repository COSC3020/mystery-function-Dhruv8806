[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11740206&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) { //mystery() function takes an array 'a' as an input.
    if(a.length == 1) return a[0]; //Checks if array 'a' has one element, it returns that element.    
    var foo = mystery(a.slice(1, a.length)) // As far as I get it. It creates 'var' foo than uses 'slice' function which is used to remove the first element from the array creating a smaller array.
    if(foo > a[0]) return foo; //If foo is greater/larger. Foo returns as the maximum
    else return a[0]; // Else it returns as first element as maximum. 
}
//Example: As I've tested this example it provides the maximum value, which is '67'
console.log(mystery([1,3,12,67,5,4]));

// Overall, this mystery function is to recursively find and return the maximum value within inputing an array.
/*
Sources used: 
Referred to TA in Lab time, as I was a bit unsure, the TA explained me a bit about "mystery" function. 
Discussed with Ziyu Wang, one of the classmates as well. 
*/
```
