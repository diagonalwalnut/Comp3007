# Comp3007

## Homework 4

### Thad Hoskins

### January 26, 2020

_______________________

### 1. Determin the intervals on which the following function is increasing/decreasing

$$f(x)=2x^{3}+3x^{2}-120x+60$$

To determine where $f(x)$ is increasing/decreasing, I will take the derivative. When $\frac{d}{dx} f(x)$ is positive, $f(x)$ is increasing. When $\frac{d}{dx} f(x)$ is negative, $f(x)$ is decreasing. First, the derivative:

$\frac{d}{dx} f(x) = 6x^2 + 6x -120$

To determine where $f(x)$ is positive or negative, I will set $\frac{d}{dx} f(x)$ equal to zero. This will give me points at which $\frac{d}{dx} f(x)$ changes from positive or negative to negative or positive, respectively.

$6x^2 + 6x -120 = 0$\
$x^2 + x - 20 = 0$\
$(x + 5)(x - 4) = 0$

Using the $\frac{d}{dx} f(x)$ above, at $x = -5$ and $x = 4$ $\frac{d}{dx} f(x)$ is zero. Next is to determine whether each interval is changing from positive to negative or negative to positive. To do so, I will select a value in each of the 3 intervals.

Sample values for $x$: $-10, 0, +10$

$\frac{d}{dx} f(-10) = 420$\
$\frac{d}{dx} f(-0) = -120$\
$\frac{d}{dx} f(10) = 540$

The interval $\frac{d}{dx} f(x)$ for $x$ values less than $-5$ are positive. Therefore $f(x)$, for $x$ values less than $-5$, $\frac{d}{dx} f(x)$ is increasing.

The interval $\frac{d}{dx} f(x)$ for $x$ values greater than $-5$ and less than $4$ are negative. Therefore $f(x)$, for $x$ values greater than $-5$ and less than $4$, $\frac{d}{dx} f(x)$ is decreasing.

The interval $\frac{d}{dx} f(x)$ for $x$ values greater than $4$ are positive. Therefore $f(x)$, for $x$ values greater than $45$, $\frac{d}{dx} f(x)$ is increasing.

### 3. Give the formula for a function that has no local maximum or minimum, but whose derivative has at least one sign change

### 4. Find the absolute minimum of the function $f(x) = x^2\ln{x}$

For the absolute minimum, I will start with finding points where the curve "bottoms out", which is to say when $f(x)$ (originally typed "it") is "concave up" and changing from negative to positive. To find both, I will take the derivative.

First, observations:\

* $x^2$ cannot be negative
* $\ln{x}$ cannot be negative
* $f(0)$ is undefined
* therefore $f(x)$ must be positive

Domain of $f(x)$ is $(0,+\infin)$

$$f(x) = x^2\ln{x}$$

To find the derivative, I will apply the product rule to the product of $x^2$ and $\ln{x}$

$$\frac{d}{dx} x^a = ax^{a-1}$$

$g(x) = x^2$\
$\frac{d}{dx} g(x) = 2x$

$$\frac{d}{dx} \ln{a} = \frac{1}{a}$$

$h(x) = \ln{x}$\
$\frac{d}{dx} h(x) = \frac{1}{x}$

$$\frac{d}{dx} [g(x)h(x)] = \frac{d}{dx} g(x)*h(x) + g(x)*\frac{d}{dx} h(x)$$

$\frac{d}{dx} f(x) = 2x*\ln{x} + x^2\frac{1}{x} = 2x\ln{x} + x$

With the derivative, I can now solve for when $\frac{d}{dx} f(x)$ = 0. This will give me the point where $f(x)$ changes from decreasing to increasing or increasing to decreasing.

$2x\ln{x} + x = 0$\
$2x\ln{x} = -x$\
$2x\ln{x} = -\frac{x}{2x}$\
$\ln{x} = -\frac{1}{2}$

Using the definitions of logs, $e^{ln x} = x$

$e^{ln{x}} = e^{-\frac{1}{2}}$\
$x = e^{-\frac{1}{2}}$

In this case, $\frac{d}{dx} f(x) = 0$ at $x = e^{-\frac{1}{2}}$.

We now have the point where $\frac{d}{dx} f(x)$ cross zero. But from what to what (i.e.. negative to positive or positive to negative?)?

Plugging in values above and below $e^{-\frac{1}{2}}$ will clear this up.

$e^{-\frac{1}{2}}$ is about $.607$, so $x = .5$ and $x = 1$ should bracket nicely.

$$\frac{d}{dx} f(x) = 2x\ln{x} + x$$

$\frac{d}{dx} f(.5) = .5 * \ln{.5} + .5 = -.193$\
$\frac{d}{dx} f(1) = 1 * \ln{1} + 1 = 1$

At $x = e^{-\frac{1}{2}}$  $\frac{d}{dx} f(x)$ changes from negative (to the left of $e^{-\frac{1}{2}}$) to positive (to the right of $e^{-\frac{1}{2}}$). This tells me that $f(x)$ in fact changes from decreasing to increasing, rather than flattening or some other shape that would result in multiple values at the bottom.

The next question is whether or not $f(x)$ is concave up or down at this point. Checking the graph, I know it is concave up, but...

To find out for sure, I can take the derivative of $\frac{d}{dx} f(x)$ to determine whether or not $f''(x)$ is positive (I do not know the notation for a derivative of a derivative, so I will sloppily swith to prime notation). If $f''(x)$ is $\bold{postive}$, then it follows that $\frac{d}{dx} f(x)$ is $\bold{increasing}$, which then means that $f(x)$ is concave $\bold{up}$.

$$\frac{d}{dx} 2x\ln{x}+x$$

$f''(x) = $\frac{d}{dx} 2x\ln{x} + \frac{d}{dx} x$\
$\frac{d}{dx} 2x\ln{x} = \frac{d}{dx} n(x)*m(x) + n(x)*\frac{d}{dx} n(x)$

$n(x) = 2x$\
$\frac{d}{dx} n(x) = 2$

$m(x) = \ln{x}$\
$\frac{d}{dx} m(x) = \frac{1}{x}$

$\frac{d}{dx} 2x\ln{x} = 2*\ln{x} + 2x*\frac{1}{x} = 2\ln{x} + 2$

$f''(x) = (2\ln{x} + 2) + 1) = 2\ln{x} + 3$

Plugging in $x = e^{-\frac{1}{2}}$ into $f''(x)$, we find that $f''(e^{-\frac{1}{2}}) = 2$ which is positive.

(In haste and tunnel vision, I solved $f''(x)$ to find where it crossed zero. Only after typing it did I realize my mistake. Oops.)

At $x = e^{-\frac{1}{2}}$ we see that:

* $f''(x)$ is positive,
* which means $\frac{d}{dx} f(x)$ is increasing,
* which means $f(x)$ is concave.

So, we know that at $x = e^{-\frac{1}{2}}$ f(x)  changes from decreasing to increasing and is $\bold{concave}$ $\bold{up}$. Because $\frac{d}{dx} f(x)$ was equal to $0$ at only 1 point, the absolute minimum of $f(x)$ is at $x = e^{-\frac{1}{2}}$. (I may be making an assumption that should not be made) I can further deduce this as $f(x)$ increases toward infinite as $x$ increases beyond $x = e^{-\frac{1}{2}}$.

The absolute minimum of f(x) is at:

$$x = e^{-\frac{1}{2}}$$
$$f(e^{-\frac{1}{2}}) = -\frac{1}{2}e^{-1}$$

For the graphs I used: <https://www.desmos.com/calculator/xwthhbld9t>

### 5. Find the absolute maximum of the function $\iota(\lambda) = \frac{\lambda^xe^{-\lambda}}{x!}$, defined on the interval $\lambda \in (0, \infin)$. Note that x is a constant while $\lambda$ is the variable

First, for typing, you are killing me on the characters for variables. Therefore...

$\lambda = l$
$\iota = i$

$\iota(\lambda) = \frac{\lambda^xe^{-\lambda}}{x!}$ then becomes $i(l) = \frac{l^xe^{-l}}{x!}$

I started this one by graphing it.

<https://www.desmos.com/calculator/sxnusbbkso>

For $x$ with a value of 0...

As $l$ increases toward $\infin$, $f(l)$ approaches $0$. The problem gives itself an interval of $l > 0$. As $l$ approaches the limit of 0, $f(l)$ approaches 1.

However, as $x$ increases, $f(l)$ changes behavior. With $x = 1$, $f(l)$, for $l$ values approaching 0, approaches 0.

Taking the derivative:

$\frac{d}{dx} f(l) = \frac{e^{-x}(l - x) x^{l - 1}}{l!}$

Using this, we can determine the patterns of increase and decrease. As $x$ increases, when $l$ increases...
