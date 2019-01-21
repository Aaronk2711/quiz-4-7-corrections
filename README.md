# quiz-4-7-corrections

## Quiz 4:

### Question 9:

My Answer: const pi = 3.14;

Correct Answer: const PI = 3.14;

First of all, you want to use the constant declaration because the number pi will not change throughout your code. And because you are using the const keyword, you have to use the naming convention for it. The nameing convention for the const keyword is UPPERCASE which means that my answer was acceptable, but not the best answer which is what the question was asking for.

### Question 10

My Answer: False, Undefined, NaN, null

Correct Answer: False, 0, Undefined, NaN, "", null

Although all of my answers were correct, they were not all the applicable ones to the question. The term falsey refers to all values, that when left by themselves, would evaluate to false. These are slightly ambiguous terms so an empty string and 0 are examples of those and therefore are correct answers. 

### Question 11

Correct Answer:

function offToCollege(){
  let favCollege = prompt("What is your favorite college?");
  let totalCost = prompt("Please enter the approximate cost of staying at " + favCollege + " for all 4 years.");
  document.getElementById("off-to-college").innerHTML = favCollege + " is a pretty expensive school! It'll cost you $" + (totalCost/4) + " per year!"
}

function carpool(){
  let friends = Number(prompt("How many friends do you want to bring to the movies?"));
  let suvAvailable = Number(prompt("How many SUVS are available for driving?"));
  let suvNeeded = Math.floor(numOfFriends/7);
  let suvs;
  let sedans;
  if(suvNeeded>suvAvailable){
    suvs = suvAvailable;
    sedans = Math.ceil((friends-(7*suvAvailable))/4);
    console.log(suvs + " parents who drive SUVs and " + sedans + " parents who drive sedans are required to transport the " + friends + " friends to the movies." ); }
    else if(suvNeeded<suvAvailable){
    suvs = suvsNeeded;
    sedans = Math.ceil((numOfFriends-(7*suvsNeeded))/4);
    console.log(suvs + " parents who drive SUVs and " + sedans + " parents who drive sedans are required to transport the " + numOfFriends + " friends to the movies." );
  }
}

## Quiz 5:

### Question 2

My Answer: >, ==, !, !==, <, =, !=, <=, ===, >=

Correct Answer: >, ==, !==, <, !=, <=, ===, >=

Most of my answers were correct. However, both ! and = were incorrect. This is because neither of them were actually comparative operators. ! is a negation and = is not used for comparing, rather for setting something equal to something else.

### Question 3

My Answer: 
x === y
x != y

Correct Answer:
x === y
x !== y

The reason that my answer is wrong is because when I only use one equal sign after the exclamation mark, I am only checking for value. However, because one of the variables is a string and the other is an integer, I need to check using two equal signs which will check for value and type of value.

### Question 4

My Answer: &&, ||, ?

Correct Answer: &&, !, ||

My first two answers were correct. However, the question mark is not a logical operator, rather more of a comparative operator. On the other hand, the exclamation mark is a logical operator because it means "not".

### Question 8

My Answer: 
switch (score) {
  case >= 90; letterGrade = "A"; break;
  case >= 80: letterGrade = "B"; break;
  case >= 70: letterGrade = "C"; break;
  case >= 60: letterGrade = "D"; break;
  default: letterGrade = "F"; break;
}


Correct Answer:
if (score >= 90) {
    letterGrade = "A";
} else if (score >= 80) {
    letterGrade = "B";
} else if (score >= 70) {
    letterGrade = "C";
} else if (score >= 60) {
    letterGrade = "D";
} else {
    letterGrade = "F";
}

The reason that this is the correct answer is because an if statement is generally simpler than a switch statement. The switch statement is arguably easier to code, but not necessarily simpler as the if statement is much more intuitive than switch.

### Question 10

My Answer: 
let status = (studentGrade >= 88)
  ? "HR"
  : "ND";
  
let status = (studentGrade >= 88) ? "HR" :
"ND";

Correct Answer:
let status = (studentGrade >= 88)
  ? "HR"
  : "ND";
  
let status = (studentGrade >= 88) ? "HR" :
"ND";

let status = (studentGrade < 88) ? "ND": "HR";

The reason that I got this question slightly incorrect is because I did not include the last answer. I do not have to check for HR first because I can just check for ND first by asking if studentGrade < 88 in the if statement. Then, if it is not ND then it will be HR. So, although my answer was partially correct, it was not completely correct. 

### Question 12

My Answer: 

do {
  x--;
} while (x > 100);

Correct Answer: 

do {
  x--;
} while (x > 100);

do {
  x++;
} while (x < 100);

Although my answer was partially correct, it did not account for all possible answers. Instead of just going from the top to the bottom, I could start from the bottom and go up and check all the values that way, which means that I only got this question partly correct. 


## Quiz 6:

### Question 1

My Answer: The name of the function is mystery, The function is designed to return a value, The function is not designed to accept any parameters

Correct Answer: Although two of my answers were correct, the one that said that the function is designed to return a value is incorrect. Although plausible for this function to return a value, not enough details have been given to concretely say so.

### Question 3

My Answer: I need to do homework, chores, and more homework... So busy!; I need to do chores, homework, and... So busy!; I need to do homework, homework, and more homework... So busy!

Correct Answer: I need to do homework, chores, and more homework... So busy!; I need to do chores, homework, and undefined... So busy!;I need to do homework, homework, and more homework... So busy!;

As in previous questons, I had two of the answers correct but only one wrong. This time, when one of the parameters was undefined, I assumed that it would not return anything and thus would be left blank in the string. However, the value was set to undefined and it was printed in the statement, making my answer incorrect.

### Question 4

My Answer:

function divide(a, b) {
    a = Number(prompt("Enter a number."));
    b = Number(prompt("Enter another number."));

    return a / b;
}

Correct Answer:

function divide(a, b) {
    return a / b;
}

My answer was incorrect because of my two statements in the function. In the definition of the function, it asks for two parameters already, which will be divided. Because of this, I do not need to prompt the user for the number. Rather, I must enter the numbers myself so that they can be divided.

### Question 15

My Answer: False

Correct Answer: True

This question asks if the declaration of a variable using var within a block effectively pushes it up to the function scope. At first I said that it was wrong but this is incorrect. The reason that I thought it was incorrect was because I thought it would go to the global scope and surpass the function scope entirely. However, I was wrong and it only went up one scope, which makes the answer true.

## Quiz 7:

### Question 4

My Answer: cars.includes(car)

Correct Answer: cars.includes(car), cars.lastIndexOf(car) !== -1, cars.indexOf(car) !== -1

Again, I got this question partially right but not completely. Although cars.includes is a fair way of determining if a value is found within an array, it is also possible to use .lastIndexOf and indexOf to determine if the index of the specific car we are looking for is even valid. This is why my answer is only partially right.


