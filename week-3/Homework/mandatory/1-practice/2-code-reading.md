# Code reading

## Question 1

Take a look at the following code:

```
1    let x = 1;
2    {
3        let x = 2;
4        console.log(x);
5    }
6    console.log(x);
```

Explain why line 4 and line 6 output different numbers.

the output from line 4 will be 2 because x is local variabl
but the output from line 6 will be 1 because x is global variable.

## Question 2

Take a look at the following code:

```
let x = 10

function f1()
{
    console.log(x)
    let y = 20
}

console.log(f1())
console.log(y)
```

What will be the output of this code. Explain your answer in 50 words or less.

the output will be 10 and undefined with an error messege shows that y is not defined becaus y is local variable iI can us it only inside the function while x is global variable.
## Question 3

Take a look at the following code:

```
const x = 9;

function f1(val) {
  val = val + 1;
  return val;
}

f1(x);
console.log(x);

const y = { x: 9 };

function f2(val) {
  val.x = val.x + 1;
  return val;
}

f2(y);
console.log(y);
```

What will be the output of this code. Explain your answer in 50 words or less.
the output of this code is 9 and {x:10}.
9 because it tokes the global variable y and us it in function f2 as a parametar the output from this function is 9.
{x:10} because it console.log a global variable y but after doing the return the value of x becomes 10.