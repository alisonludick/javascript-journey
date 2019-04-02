# My Javascript Journey

I set out to focus on JavaScript fundamentals and this comes from the book You Don't Know JS: Up and Going. Such an excellent resource!
At the end of the first chapter, a challenge was set to write a program that calculated the total price of a cell phone, accessories and to include tax in that calculation; and also bare in mind the limitation of your bank balance. 
The solution is way better than mine, and I'd encourage to work through the book on your own to see it; but here is my attempt at writing that program:

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
