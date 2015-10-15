# Haskell-Car-Validator
Haskell Credit Card validator exercise (my solution :) ) 

```
The algorithm follows these steps:

Double the value of every second digit beginning with the rightmost.
Add the digits of the doubled values and the undoubled digits from the original number.
Calculate the modulus of the sum divided by 10.
If the result equals 0, then the number is valid. Here is an example of the results of each step on the number 4012888888881881.

In order to start with the rightmost digit, we produce a reversed list of digits. Then, we double every second digit. 
Result: [1,16,8,2,8,16,8,16,8,16,8,16,2,2,0,8].

We sum all of the digits of the resulting list above. Note that we must again split the elements of the list into their digits (e.g. 16 becomes [1, 6]).
Result: 90.

Finally, we calculate the modulus of 90 over 10.
Result: 0.

Since the final value is 0, we know that the above number is a valid credit card number. If we make a mistake in typing the credit card number and instead provide 4012888888881891, then the result of the last step is 2, proving that the number is invalid.
```
