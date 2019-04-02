# My Javascript Journey

I set out to focus on JavaScript fundamentals and this comes from the book [You Don't Know JS: Up and Going](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch1.md). Such an excellent resource!  

At the end of the first chapter, a challenge was set to write a program that calculated the total price of a cell phone, accessories and to include tax in that calculation; and also bare in mind the limitation of your bank balance.   

The solution is way better than mine, and I'd encourage to work through the book on your own to see it; but here is my attempt at writing that program:  

In the first 4 lines I declared the *variables* I needed in my program, namely, *taxRate*, *phonePrice*, *accessPrice* and *bankBal*.  

The following 2 lines I included after I wrote the program to see whether an increase in price would affect the message that was included with each condition. And it did!  

The program itself reads:  
>To calculate the total amount spent...  
>add the total price of the phone and accessories together with the tax included on top of that sum  
>and return the answer as an asbolute value of a number, rounded up to 2 decimal places  
>If that amount is less than or equal to what's in the bank  
>then include the message `"I can afford this purchase :)"`  
>else use the message `"I don't have enough money for :("`

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
