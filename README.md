# PrimeNumbers



### _Assumptions_

 - Is it correct that 1 is not considered a prime number? Y
 - Can I assume that the entries are valid? N
 - Can I assume that this fits the memory? Y
 
 
 
### _Test Cases_

 - None -> Exception
 - Not an int -> Exception
 - 20 -> [False, False, True, True, False, True, False, True, False, False, False, True, False, True, False, False, False, True, False, True]



## Algorithm


_For a number to be prime, it must be 2 or greater and cannot be divisible by a number other than itself (and 1)._

All non-prime numbers are divisible by a prime number.

 - Use an array to keep track of each integer to the maximum
 - Start at 2, end at sqrt (max). I can use sqrt (max) instead of max because: 
      For each value that divides the input number evenly, there is a complement b where ab = n.
      If a> sqrt (n) then b <sqrt (n) because sqrt (n ^ 2) = n.
      
 "Cross off" all numbers divisible by 2, 3, 5, 7, ... by setting array [index] to False.
