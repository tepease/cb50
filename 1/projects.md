## Unit 1 

In this unit we'll be getting familiar with C syntax. 
You'll learn what your Scratch 'control' puzzle pieces are in the C language, and become comfortable with using them. 

######Reminder: in all code snippets, user input is denoted with *asterisks\*. Anything in *asterisks\* should be entered by you at the command line while your program is running.


### Projects

#### <a name='echo'></a> echo

Write a program that takes input and echoes it back, just like the below snippet.
```
~/workspace/ $ ./echo
go on, yell: *foo!*
foo!
~/workspace/ $ ./echo
go on, yell: *bar!*
bar!
~/workspace/ $
```


#### <a name='scream'></a> scream

```
~/workspace/ $ ./scream
how scary, as a number? *5*
aaaaah!
~/workspace/ $ ./scream
how scary, as a number? *3*
aaah!
~/workspace/ $
```


#### <a name='s_p_l_i_t'></a> s_p_l_i_t

```
~/workspace/ $ ./split
word to split: *myword*
m y w o r d
~/workspace/ $
```

#### <a name='grid'></a> grid

```
~/workspace/ $ ./grid
size: *3*
@@@
@@@
@@@
~/workspace/ $ ./grid
size: *2*
@@
@@
~/workspace/ $
```

#### <a name='numgrid'></a> numgrid.c

```
~/workspace/ $ ./numgrid
size: *3*
012
123
234
~/workspace/ $ ./numgrid
size: *2*
01
12
~/workspace/ $
```


#### <a name='takes2'></a> takes2.c

```
~/workspace/ $ ./takes2
size: *3*
  2
 2 
2  
~/workspace/ $ ./takes2
size: *2*
  
 2
~/workspace/ $
```

#### <a name='steps'></a> steps.c

```
~/workspace/ $ ./steps
size: *3*
  _
 _ 
_  
~/workspace/ $ ./steps
size: *2*
  
 _
~/workspace/ $
```


#### <a name='esrever'></a> esreveR.c

```
~/workspace/ $ ./esrever
word please: *hello*
olleh
~/workspace/ $
```


#### <a name='choosy.c'></a> choosy.c
Prompt for a number, and take it with getString(). If any character is not a digit, prompt again.
```
~/workspace/ $ ./choosy
number please: *hi*
that's not a number...
number please: *7*
nice 7, thanks!
~/workspace/ $
```

#### <a name='strint'></a> strint.c

Take string input and print out the integer value of each character, in order
```
~/workspace/ $ ./strint
word please: *abcd*
97 98 99 100
~/workspace/ $
```


#### <a name='tenner'></a> tenner.c

Take number input and print out the digit in the tens place. If the number is less than 10, print 0.
See if you can do this using get_string(), then see if you can do it with get_int().
```
~/workspace/ $ ./tenner
un nombre, sil vous plait: *1290*
9
~/workspace/ $ ./tenner
un nombre, sil vous plait: *129*
2
~/workspace/ $
```

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