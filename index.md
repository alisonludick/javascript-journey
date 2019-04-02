# My Javascript Journey

I just wrote my first piece of code and I'm wondering if this is the correct way to publish it:

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
