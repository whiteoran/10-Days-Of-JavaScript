# 10-Days-Of-JavaScript
Hackerrank 10 days of javascript solution



// Day 0: Hello, World!

function greeting(parameterVariable) {
    // This line prints 'Hello, World!' to the console:
    console.log('Hello, World!');
    console.log(parameterVariable)

    // Write a line of code that prints parameterVariable to stdout using console.log:

}


// Day 0: Data Types

function performOperation(secondInteger, secondDecimal, secondString) {
    // Declare a variable named 'firstInteger' and initialize with integer value 4.
    const firstInteger = 4;

    // Declare a variable named 'firstDecimal' and initialize with floating-point value 4.0.
    const firstDecimal = 4.0;

    // Declare a variable named 'firstString' and initialize with the string "HackerRank".
    const firstString = 'HackerRank ';

    console.log(firstInteger + parseInt(secondInteger))

    console.log(firstDecimal + parseFloat(secondDecimal))

    console.log(firstString + secondString)
}

//Day 1: Arithmetic Operators

function getArea(length, width) {
    let area;
    // Write your code here
    area = length * width;
    
    return area;
}

function getPerimeter(length, width) {
    let perimeter;
    // Write your code here
    perimeter = 2 * (length + width);
    return perimeter;
}

//Day 1: Functions

function factorial(n){
    if(n==0)
        return 1;
        else
        return n * factorial(n-1); 
    }
    
    
//Day 1: Let and Const

function main() {
let r = readLine();
const PI = Math.PI;

// Print the area of the circle:
console.log(PI*r*r);
// Print the perimeter of the circle:
console.log(PI*2*r);

// Day 2: Conditional Statements: If-Else

function getGrade(score) {
    let grade;
    // Write your code here
    if (score > 25 && score <= 30) grade = "A"
    else if (score > 20 && score <= 25) grade = "B"
    else if (score > 15 && score <= 20) grade = "C"
    else if (score > 10 && score <= 15) grade = "D"
    else if (score > 5 && score <= 10) grade = "E"
    else if (score >= 0 && score <= 5) grade = "F"
    return grade;
    
 //Day 2: Conditional Statements: Switch
 
 function getLetter(s) {
    switch(s[0]) {
        case 'a':
        case 'e':
        case 'i':
        case 'o':
        case 'u':
            return 'A';
        case 'b':
        case 'c':
        case 'd':
        case 'f':
        case 'g':
            return 'B';
        case 'h':
        case 'j':
        case 'k':
        case 'l':
        case 'm':
            return 'C';
        default:
            return 'D';
    }
}


//Day 2: Loops


function vowelsAndConsonants(s) {
    const vowels = 'aeiou';
    var consonants = '';
    
    for(var i = 0; i < s.length; i++) {
       if (vowels.includes(s[i])) {
           console.log(s[i]);
       }
       else {
           consonants += s[i] + '\n';
       }
    }
    
    console.log(consonants.trim());
}

//Day 3: Arrays

function getSecondLargest(nums) {
    let largest = nums[0];
    let secondLargest = nums[0];
    
    for (let i = 1; i < nums.length; i++) {
        if (nums[i] > largest) {
            secondLargest = largest;
            largest = nums[i];
            continue;
        }
        
        if ((nums[i] > secondLargest) && (nums[i] < largest)) {
            secondLargest = nums[i];
        }
    }
    
    return secondLargest;
}

// Day 3: Try, Catch, and Finally

/*
 * Complete the reverseString function
 * Use console.log() to print to stdout.
 */
function reverseString(s) {
    try {
        s = s.split('').reverse().join('');
    }
    catch (e) {
        console.log(e.message)
    }
    finally {
        console.log(s)
    }
}


// Day 3: Throw

function isPositive(a) {
    if (a <= 0) {
        throw (a === 0 ? new Error("Zero Error") :
            new Error("Negative Error"))
    }
    else {
        return "YES"
    }
}

//Day 4: Create a Rectangle Object

function Rectangle(a, b) {
    this.length = a;
    this.width = b;
    this.perimeter = 2 * (a+b);
    this.area = a*b;
}

//Day 4: Count Objects

function getCount(objects) {
return objects.filter(item =>item.x===item.y).length;
}

//
