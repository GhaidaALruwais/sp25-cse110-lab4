1. What was the bug? num1 and num2 were being treated as strings. So "2" + "3" returned "23" instead of performing numeric addition
2. How would you fix it? convert both inputs into numbers before adding them
function calculateSum(num1, num2) {
  let result = Number(num1) + Number(num2);
  return result;
}