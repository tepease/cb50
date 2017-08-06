#### <a name='choosy.c'></a> choosy.c
Prompt for a number, and take it with getString(). If any character is not a digit, prompt again.

#### <a name='esrever'></a> esreveR.c
Take string input and print it out ... backwards

#### <a name='takes2'></a> takes2.c
Implement numgrid.c from above, but ONLY print the number 2

#### <a name='tenner'></a> tenner.c
Take number input and print out the digit in the tens place. If the number is less than 10, print 0.

#### <a name='strint'></a> strint.c
Take string input and print out the integer value of each character, in order

#### <a name='pin'></a> PIN sequence
Here are a series of ATM PIN checking algorithms for you to implement. 
Numbered 1 through 5, they start simple and get progressively more advanced. 
I'll post only my console output, and you sort out how to replicate it. 
Before starting each, identify exactly how it differs from the one before,
and reuse any code you can in each iteration.
Remember to compile and run after each change you make so you don't get into any rabbit holes!
 
 ```
 ~/workspace/ $ make pin1
 clang -fsanitize=integer -fsanitize=undefined -ggdb3 -O0 -std=c11 -Wall -Werror -Wextra -Wno-sign-compare -Wshadow    pin1.c  -lcrypt -lcs50 -lm -o pin1
 ~/workspace/ $ ./pin1
 pin: 1
 pin: 0000
 pin: banana
 Retry: mugs
 Retry: 922
 pin: 10000
 pin: 9876
 pin: 1234
 correct!
 ~/workspace/ $ 
 ```
 
 ```
 ~/workspace/ $ make pin2
 clang -fsanitize=integer -fsanitize=undefined -ggdb3 -O0 -std=c11 -Wall -Werror -Wextra -Wno-sign-compare -Wshadow    pin2.c  -lcrypt -lcs50 -lm -o pin2
 ~/workspace/ $ ./pin2
 pin: 1
 your pin must have 4 digits
 pin: 0000
 your pin must have 4 digits
 pin: banana
 Retry: mugs
 Retry: 922
 your pin must have 4 digits
 pin: 10000
 your pin must have 4 digits
 pin: 9876
 pin: 1234
 correct!
 ~/workspace/ $ 
 ```
 
 ```
~/workspace/ $ make pin3
clang -fsanitize=integer -fsanitize=undefined -ggdb3 -O0 -std=c11 -Wall -Werror -Wextra -Wno-sign-compare -Wshadow    pin3.c  -lcrypt -lcs50 -lm -o pin3
~/workspace/ $ ./pin3
pin: 1
your pin must have 4 digits
pin: 0000
your pin must have 4 digits
pin: banana
Retry: mugs
Retry: 10000
your pin must have 4 digits
pin: 9876
incorrect, try again
pin: 1234
correct!
~/workspace/ $ 
```

```
~/workspace/ $ make pin4
clang -fsanitize=integer -fsanitize=undefined -ggdb3 -O0 -std=c11 -Wall -Werror -Wextra -Wno-sign-compare -Wshadow    pin4.c  -lcrypt -lcs50 -lm -o pin4
~/workspace/ $ ./pin4
pin: 1
your pin must have 4 digits
pin: 0000
incorrect, try again
pin: banana
your pin must have 4 digits
pin: mugs
incorrect, try again
pin: 10000
your pin must have 4 digits
pin: 9876
incorrect, try again
pin: 1234
correct!
~/workspace/ $
```

```
~/workspace/ $ make pin5
clang -fsanitize=integer -fsanitize=undefined -ggdb3 -O0 -std=c11 -Wall -Werror -Wextra -Wno-sign-compare -Wshadow    pin5.c  -lcrypt -lcs50 -lm -o pin5
~/workspace/ $ ./pin5
pin: 1
your pin must have 4 digits
pin: 0000
incorrect, try again
pin: banana
your pin must be numbers only
pin: mugs
your pin must be numbers only
pin: 10000
your pin must have 4 digits
pin: 9876
incorrect, try again
pin: 1234
correct!
~/workspace/ $
```