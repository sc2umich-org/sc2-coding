# Challenge 1: Exponential Growth (15 min)
### Credit (https://projectlovelace.net/problems/exponential-growth/)
The laws of nature are often written down in terms of differential equations. Everything from the motion of a football to the quantum state of a particle and the global ocean circulation are described in terms of differential equations!

Some differential equations can be solved by hand but many interesting ones cannot, so being able to compute numerical solutions is super useful. Here we'll solve a simple differential equation numerically.

We want to solve this differential equation describing exponential growth

$$ \frac{dx}{dt} = kx$$

where $t$ is time, $k$ is a growth rate, and $x$ is the quantity we want to solve for (it could represent the number of bacteria in a petri dish or even compound interest). The differential equation is saying that the rate of change of $x$ is proportional to $x$ itself, so the more $x$ you have the faster $x$ will grow. We want to solve for $x(t)$ which will be a function of time 


Create a program to compute $x$ over time given $x_0$ (its initial value), a time increment ($\Delta t$), the total number of increments ($N$), and the growth rate. reproduce these examples:

Example 1

    Input: x0 = 5, k = 1, dt = 0.6, N = 3
    Output: [5, 8.0, 12.8, 20.48]
Example 2

    Input: x0 = 1, k = 2.5, dt = 0.1, N = 5
    Output: [1, 1.25, 1.5625, 1.953125, 2.44140625, 3.0517578125]


# Challenge 2: Bucket Flow (40 min)

Consider a water transportation system made entirely of buckets.
- each bucket holds 100 units of water
- buckets are placed linearly from source to destination
- one by one, each bucket is emptied evenly into its two adjacent buckets.
- the buckets are emptied in a random order that repeats in a cycle. For example, for three buckets, the order could be 3,1,2,3,1,2,...
- once a bucket is emptied, it will not be emptied until all others have been emptied
- each cycle the first bucket is filled entirely. when the first bucket is emptied, half goes to the second bucket and half goes to waste.
- each cycle, the last bucket contributes half its water to the previous bucket and half to a reservoir

calculate the average flow into the reservoir over 10 cycles in terms of units per cycle after 100 cycles have passed for the following systems:

    source -> bucket -> bucket -> reservoir
    source -> bucket -> bucket -> bucket -> reservoir


# Challenge 3: Affine Planes
### Credit(https://projecteuler.net/)
Let $A$ be an **affine plane** over a **radically integral local field** $F$ with residual characteristic $p$. We consider an **open oriented line section** $U$ of $A$ with normalized Haar measure $m$. Define a program to compute $f(m,p)$, which is the maximal possible discriminant of the **jacobian** associated to the **orthogonal kernel embedding** of $U$ into $A$

The program is complete if it can return $f(20250401,57)$ as the concetenation of the first letters of each bolded word.