# Comp3007

## Homework 3

### Thad Hoskins

### January 19, 2020

_______________________

### 4. Each of the following is Big-O of what functions

a. The time it takes to print the first item on a list when the list is $\textit{n}$ items long.

The first item is always going to be item [0]. It does not matter how many items there are (ignoring memory and processing). Therefore Big-O notation is

$$O(1)$$

b. The time is takes to print all items on a list when the list is $\textit{n}$ items long.

In this case, the amount of time it takes is specifically dependent on how many ($\textit{n}$) items there are. It is linear. Therefore the Big-O notation is

$$O(n)$$

c. The time it takes to print all ordered pairs (n$_1$, n$_2$) of items from the list when the list is $\textit{n}$ items long.

For each value in n$_1$, one would need to loop through n$_2$. The current value of n$_1$ is then compared to the current value of n$_2$. That is to say, one would loop through n$_2$ n$_1$ times to compare every value against every other value. That give a Big-O notation of

$$O(n^2)$$

### 6. Find the derivative of each of the following functions

d. $f(x) = \frac{e^{bx}}{1+e{bx}}$

$f(x) = \frac{g(x)}{h(x)}$

$g(x) = e^{bx}$\
$h(x) = 1 + e^{bx}$

To take the derivative of $g(x)$, I want to use $a^x$, but cannot as $\textit{bx}$ is not $\textit{x}$. Therefore, the chain rule will be used.

$i(x) = bx$\
$\frac{d}{dx} i(x) = b$
_______________________
$g(i(x)) = e^{bx}$\
$\frac{d}{dx} g(x) = a^x*ln(a)$\
$\frac{d}{dx} g(x) = e^{x}*ln e$
_______________________
$\frac{d}{dx} g(i(x)) = \frac{d}{dx} g(i(x))*\frac{d}{dx} i(x)$\
$\frac{d}{dx} g(i(x) = (e^{bx}*ln e)*b = e^{bx}*b$
_______________________
$h(x) = 1 + e^{bx}$ \
$h(i(x)) = 1 + e^{bx}$ \
$\frac{d}{dx} h(x) = 0 + a^x*ln(a)$

$\frac{d}{dx} h(x) = e^{x}*ln e$
_______________________
$e^{bx}$ from $g(x)$ is the same, so using $i(x)$... \
$\frac{d}{dx} h(i(x)) = \frac{d}{dx} h(i(x))*\frac{d}{dx} i(x)$ \
$\frac{d}{dx} h(i(x) = (e^{bx}*ln(e))*b = e^{bx}*b$

And back to the beginning...\
$f(x) = \frac{g(x)}{h(x)}$\
$\frac{d}{dx} f(x) = \frac{\frac{d}{dx} g(x)*h(x)+g(x)*\frac{d}{dx}h(x)}{h(x)^2} = \frac{be^{bx}*(1+e^{bx})-e^{bx}*be^{bx})}{(e^{bx})^2}$

Simplifying...\
$\frac{be^{bx}+be^{2bx}-be^{2bx})}{(e^{bx})^2}$ =

$$\frac{be^{bx}}{(e^{bx}+1)^2}$$

e. $f(b) = \frac{e^{bx}}{1+e{bx}}$

$g(b) = e^{xb}$\
$h(b) = 1 + e^{xb}$

To take the derivative of $g(b)$, I want to use $a^b$, but cannot as $\textit{bx}$ is not $\textit{b}$. Therefore, the chain rule will be used.

$i(b) = xb$\
$\frac{d}{db} i(b) = x$

_______________________

$g(i(b)) = e^{xb}$\
$\frac{d}{db} g(b) = a^b*ln(a)$\
$\frac{d}{db} g(b) = e^{b}*ln e$
_______________________
$\frac{d}{db} g(i(b)) = \frac{d}{db} g(i(b))*\frac{d}{db} i(b)$\
$\frac{d}{db} g(i(b) = (e^{xb}*ln e)*x = e^{xb}*x$
_______________________
$e^{bx}$ from $g(b)$ is the same, so using $i(b)$... \
$\frac{d}{db} h(i(b)) = \frac{d}{db} h(i(b))*\frac{d}{db} i(b)$ \
$\frac{d}{db} h(i(b) = (e^{xb}*ln(e))*x = e^{xb}*x$

And back to... Nevermind. Copy and pasting.\
$\frac{d}{db} f(b) = \frac{\frac{d}{db} g(b)*h(b)+g(b)*\frac{d}{db}h(b)}{h(b)^2}$ = $\frac{xe^xb*(1+e^{xb})-e^{xb}*xe^{bx}}{(1+e^{xb})^2}$

Simplifying...\
$\frac{xe^{bx}+xe^{2bx}-xe^{2xb}}{(e^{bx})^2}$ =

$$\frac{d}{db}f(b) = \frac{xe^{bx}}{(1+e^{bx})^2}$$

Given that all things were the same between $d)$ and $e)$ (i.e., the equation was not $bx^2$), it could have been inferred that the $x$ and $b$ could have simply been swapped between the two solutions.

### 9. Find the derivative of $f_k(x) = \sum_{n=0}^k \frac{x^n}{n!}$

$f_k(x)$ = $\sum_{n=0}^k \frac{x^n}{n!}$

Taking the first 4 terms plus the end...\
$f_k(x) = \sum_{n=0}^k \frac{x^n}{n!}$ = $\frac{1}{1}$ + $\frac{x}{1}$ + $\frac{x^2}{2}$ + $\frac{x^3}{9}$ + ... +  $\frac{x^{k-1}}{{k-1}!}$ + $\frac{x^{k}}{{k}!}$\
$\frac{d}{dx}f(x) = 0 + 1 + \frac{2x}{2} + \frac{3x^2}{6}$ + ... + $\frac{(k-1)*x^{k-1-1}}{(k-1)!}$ + $\frac{(k)*x^{k-1}}{(k)!}$ = 0 + 1 + $\frac{2x}{2} + \frac{3x^2}{6}$ + ... + $\frac{x^{k-2}}{(k-2)!}$ + $\frac{x^{k-1}}{(k-1)!}$

$\frac{d}{dx}f(x) = \sum_{n=0}^k \frac{x^{n-1}}{(n-1)!}$

***As discussed in class***

The first term (n=0, $x^{0-1}$) is not $x^{-1}$ nor does $x!$ make sense.

So, going back to the original equation, we take the $\frac{1}{1}$ out as a constant. However, doing so means the summation begins with $n=1$.

$f_k(x) = 1 + \sum_{n=1}^k \frac{x^n}{n!}$ = $1$ + $\frac{x}{1}$ + $\frac{x^2}{2}$ + $\frac{x^3}{9}$ + ... +  $\frac{x^{k-1}}{{(k-1)}!}$ + $\frac{x^{k}}{{k}!}$

The derivative is now...
$\frac{d}{dx}f(x) = 0 + \sum_{n=1}^k \frac{x^{n-1}}{(n-1)!}$ =

$$\sum_{n=1}^k \frac{x^{n-1}}{(n-1)!}$$\

(thank you for the insight in your feedback)

$f_k(x) = \sum_{n=0}^k \frac{x^n}{n!}$ = $1$ + $\frac{x}{1}$ + ... +  $\frac{x^{k-1}}{{(k-1)}!}$ + $\frac{x^{k}}{{k}!}$

When taking the derivative, the final simplified formula is then the 2nd to last sum, essentially dropping the last sum.

$f_k(x) = \sum_{n=0}^k ... \frac{x^{k-1}}{{(k-1)}!}$ $\bcancel{+ \frac{x^k}{k!}}$

$\frac{d}{dx} f(x) = \sum_{n=1}^k \frac{x^{k-1}}{{(k-1)}!}$

Am I right in the above? So, the main different between f(x) and $\frac{d}{dx} f(x)$ is dropping the finan term from $f(x)$ and $n=0$ -> $n=1$?

### 10. Find the derivative of $f_k(x) = \sum_{n=0}^\infin \frac{x^n}{n!}$, assuming that you can diffferentiate an ininite sum term-wise. Based on its derivative, can you guess what function $f(x)$ is?

As done in class:\
The derivative of $\sum_{n=1}^\infin \frac{x^{n-1}}{(n-1)!}$ is $\sum_{n=1}^\infin \frac{x^{n-1}}{(n-1)!}$

Another expression that has this same behavior is:\
$\frac{d}{dx} e^x = e^x$

It could then be inferred...

$$e^x = \sum_{n=0}^\infin \frac{x^{n-1}}{(n-1)!}$$

I checked this on Desmos. It holds.

To move from #9 to #10 is the same process. In writing out the summation, there is no "final" term to be dropped.

### 11. Find derivative of $f(p) = \ln{(\prod_{i=1}^{b} p^{xi}*(1-p)^{1-x_i})}$. Simplify using the laws of logarithms before differentiating. Note that the values $x_i$ should be treated as unknown constants, while p is the variable of differentiation

$f(p) = \ln{(\prod_{i=1}^{b} p^{xi}*(1-p)^{1-x_i})}$

Using Law of Logariths, we convert the natural log of a products to the sum of a natural log:\
$f(p) = \sum_{i=1}^{b} \ln{(p^{xi}*(1-p)^{1-x_i})}$

Then, with natural logs of products, we separate the products into sums:

$f(p) = \sum_{i=1}^{b} \ln{p^{xi}} + \sum_{i=1}^{b} \ln{(1-p)^{1-x_i}}$

I then used the Power Rule for both sums\

$$\ln{r^t} = t \ln{r}$$

$f(p) = \sum_{i=1}^{b} x_iln(p) + \sum_{i=1}^{b} (1-{x_i})\ln{(1-p)}$

Then summation of a constant:\

$$\sum_{i=1}^n ci = c\sum_{i=1}^n i$$

$f(p) = x_i \sum_{i=1}^{b} \ln{p} + (1-x_i)\sum_{i=1}^{b} \ln{(1-p)}$

Using the two parts of the sums to take the derivative, I will use $g(p)$ and $h(p)$ respectively...\

$g(p) = x_i \sum_{i=1}^{b} \ln{p}$\
$h(p) = ({1-x_i})\sum_{i=1}^{b} \ln{(1-p)}$

using the formula for the derivative of $\ln{a}$

$$\ln{a} = \frac{1}{a}$$
so$\dots$
$\frac{d}{dp} g(x) = x_i\sum_{i=1}^{b} \frac{1}{p}$

To take the derivative of $h(p)$ I use the chain rule, as $\ln{1-x}$ does not fit $'ln{a}.

$h(p) = ({1-x_i})\sum_{i=1}^{b}\ln(p)$\
$i(p) = (1-x)$\
$\frac{d}{dp} i(p) = -1$

For $\frac{d}{dp} I use:$

$$\frac{d}{da} \ln{a} = \frac{1}{\ln{a}}$$

$\frac{d}{dp} h(i(p) = ({1-x_i})\sum_{i=1}^{b} \frac{1}{1-p}*-1 = ({1-x_i})\sum_{i=1}^{b} -\frac{1}{1-p}$

Putting $g(x)$ and $h(x)$ together...\
$\frac{d}{dp} f(x) = x_i\sum_{i=1}^{b} \frac{1}{p} - ({1-x_i})\sum_{i=1}^{b} \frac{1}{1-p}$

Using the sums, as there are no $i$ or $b$ variables in the equation

$\sum_{k=1}^{n}$ $x$ = $x + x + ... x$ (nth time)

therefore $\sum_{k=1}^{n} x = nx$

$$\frac{d}{dp} f(x) = \frac{x_ib}{p} - \frac{({1-x_i})b}{1-p}$$
