# My Javascript Journey

After creating my [first page](https://alisonludick.github.io/) with the obejective of practicing CSS and HTML with a little bit of JavaScript, I felt like I needed to become grounded in JavaScript fundamentals. It wasn't really benefitting me, long term, to be able to write code but not to be able to talk about the syntax or the semantics of the code. 

After completing Zubin Pratap's course called [Before you learn programming: what will help you succeed](https://www.udemy.com/how-not-to-quit-coding/), I was convinced that was the right decision to make. For those who are self-taught, like I am, his course unpacked the critical importance of asking the right questions, for instance, 
>instead of asking, "what language should I learn", you should be asking "how do you program a computer"  

and from there choose a language that develops your understanding of programming fundamentals.  
His course left me with so much more than! He went through how to create learning goals (with the five W's): 
- Why
- What
- Where
- Who
- When   
how to manage the mental and emotional strain that comes with learning to code, and much, much more.  
I *highly* recommend this course, not only for self-taught coders, but anyone who desires to make effective decisions in life.  

### What and Where
With that in mind, the first course I chose was Coursera's [Programming Foundations with JavaScript, HTML and CSS](https://www.coursera.org/learn/duke-programming-web/home/welcome) from Duke University.  


The second resource, which compliments my learning in a great way and has been equally invaluable, is Kyle Simpson's book [You Don't Know JS: Up and Going](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch1.md). It is exceptionally well-written, easy to understand, and explains concepts very clearly.    

At the end of the first chapter, a challenge was set to write a program that calculated the total price of a cell phone, accessories and to include tax in that calculation; and also bare in mind the limitation of your bank balance.   

The solution in the book is much better than mine, and I'd encourage to work through the book on your own to practice it; but here is my attempt at writing that program:  

In the first 4 lines I declared the *variables* I needed in my program, namely:
>*taxRate*,
>*phonePrice*,
>*accessPrice*,
>*bankBal*  

The following 2 lines I included after I wrote the program to see whether an increase in price would affect the message that was included with each condition. And it did!  

The program itself reads:  
>To calculate the total amount spent...  
>add the total price of the phone and accessories together with the tax included on top of that sum,  
>and return the answer as the asbolute value of a number, rounded up to 2 decimal places.  
>If that amount is less than or equal to what's in the bank,  
>then include the message `"I can afford this purchase :)"`;  
>else use the message `"I don't have enough money :("`.

And in JavaScript code is expressed as:  

```
var taxRate = 0.08
var phonePrice = 120.75
var accessPrice = 50.89
var bankBal = 500.50

phonePrice = phonePrice * 3;
accessPrice = accessPrice * 3;

function totalSpend() {
    var spend = (phonePrice + accessPrice) + ((phonePrice + accessPrice) * taxRate) ; 
    console.log("$"+ Math.abs(spend.toFixed(2)));
    if (spend <= bankBal) {
        return "I can afford this purchase :)"; 
        } else {
            return "I don't have enough money :("; 
            }
}
```
