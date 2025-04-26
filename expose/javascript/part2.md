1. What will happen at line 12 and why? If the code causes an error, explain why. it prints "3" because i is declared as var which is accessible outside the block. also it is 3 because we exit the for loop when i equals 3
2. What will happen at line 13 and why? If the code causes an error, explain why. "150" because it is declared with var which is function scoped and each time we run the loop we overwrite it with the new value. the last time we run the loop discounted price = 300 * (1- 0.5) = 150
3. What will happen at line 14 and why? If the code causes an error, explain why. it prints "150" because the discounted price was 150 times 100 divided by 100 is 150
4. What will this function return? Give a brief explanation why. If the code causes an error, explain why. this function will return an array [50, 100, 150] because we pushed the discounted price to the stack at each iteration of the for-loop
5. What will happen at line 12 and why?  If the code causes an error, explain why. we will have an error because let makes i only accessible in the for-loop block. trying to access it out of the for loop causes an error
6. What will happen at line 13 and why? If the code causes an error, explain why. we will have an error because let makes discountedPrice only accessible in the for-loop block. trying to access it out of the for loop causes an error
7. What will happen at line 14 and why? If the code causes an error, explain why. it will print "150" because final price is defined in the function and the console call is in the function so it can access it. the value of final price is 150 because it started as 0 but in every iteration of the for loop it was overwritten. the last iteration it was overwritten by 150 times 100 divided by 100 which equals 150
8. What will this function return? Give a brief explanation. If the code causes an error, explain why. it will return [50, 100, 150] because discounted is defined in the function so the return statement can access it
9. What will happen at line 11 and why? If the code causes an error, explain why. i is declared inside the for-loop using let which makes it block scoped. so at line 11 we can't access i and we will have an error because i is not defined
10. What will happen at line 12 and why? If the code causes an error, explain why. it will print "3" because length is a constant that can be accessible throughout the function. we didn't try to overwrite the constant so we dont have any error here. 
11. What will this function return? Give a brief explanation. If the code causes an error, explain why. it will return [50, 100, 150] because although it was defined as a constant it can still be mutable with discounted.push however we cant reassign it discounted = [70, 10, ...]
12. Given the above Object, write the notation for:  (These should be in your part2.md)
    1. Accessing the value of the name property in the student object --> student.name
    2. Accessing the value of the Grad Year property in the student object --> student['Grad Year'] 
    3. Calling the function for the greeting property in the student object --> student.greeting()
    4. Accessing the name property of the object in the Favorite Teacher property in student --> student['Favorite Teacher'].name
    5. Access index zero in the array of the courseLoad property of the student object student.courseLoad[0]
 13. Arithmetic
    1. '3' + 2 --> '32' because + after a string perform string concatenation 
    2. '3' - 2 --> 1 because the - triggers numeric coercion and '3' is turned to 3 
    3. 3 + null --> 3 because null is coerced into 0 so 3 + 0 is 3
    4. '3' + null --> '3null' because + after a string perform string concatenation
    5. true + 3 --> 4 because true is coerced into 1 
    6. false + null --> 0 because false and null are coerced to 0
    7. '3' + undefined --> '3undefined' because + after a string perform string concatenation
    8. '3' - undefined --> NaN because '3' is coerced to 3, but undefined cannot be converted to a number, so the result is Not a Number
 14. Comparison
     1.  '2' > 1 --> true because '2' is a string, but when compared to a number, JavaScript does numeric coercion, so '2' becomes 2, and 2 > 1 is true
     2.  '2' < '12' --> false because Both operands are strings, so this is a lexicographic comparison (like dictionary order). '2' comes after '1', so '2' < '12' is false.
     3.  2 == '2' --> true because == allows type coercion, so '2' is converted to number 2, and 2 == 2 is true.
     4.  2 === '2' --> false because === checks for strict equality, meaning both value and type must match. Here, 2 is a number and '2' is a string → different types, so the result is false
     5.  true == 2 --> false because true is coerced to 1, so the comparison becomes 1 == 2, which is false.
     6.  true === Boolean(2) --> true because Boolean(2) returns true because any non-zero number is truth. So this becomes true === true, which is true
 15. Explain the difference between the == and === operators. === checks if the values are equal AND of the same type. No type conversion happens. in === we can do type conversions
 16. In the part2-question16.js file
 17. If the function above is called with the following parameters modifyArray([1, 2, 3], doSomething), what will be the result? Briefly walk through how you arrived at that result. the result is [2, 4, 6] The modifyArray function applies the doSomething callback (which doubles a number) to each element in the array [1, 2, 3]. So it returns a new array with each number doubled: [1*2, 2*2, 3*2] → [2, 4, 6].
 1.  In the part2-question18.js file
 2.  What is the output of the above code? 1 4 3 2