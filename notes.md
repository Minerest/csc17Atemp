notes
2/15/17
Calculating numbers in different bases.
The digit can only be as high as 1 less than the base.
For instance, something in base 16 has 0-9-A-F
0-9 makes 10 separate numbers plus A-B-C-D-E-F makes 16 numbers total.
Each time a number is 1 character longer, the next digit can be as great as 1 - the base squared.
i.e. in the 10's place in base 10, the number can only go as high as 99 or 10^2-1.
in base 16, if the number has 2 characters, then the second place can go as high as 16^2 - 1 or 255

When converting a number from base 10, you have to pay attention to how the original number relates.
if the number is below 16, then it only needs 1 character. If it's between 16 and 255,
 then you need to mod(%) the number by 16 to get the second character and the leftovers go to the first digit.

example
converting 20 in base 10 to a number in base 16, you have to find out if the number is greater than 16, 256, 16^3... etc
in this case, 20 is between 16 and 256 
so you divide by 16. 16 goes into 20 once so the first digit in base 16 is going to be 1
There's 4 leftover so 20 in base 10 is 14 in base 16
