# Github repo for lecture of analysis of algorithms


### History Bit

- FIrst mechanical computers were difference engine, and analytical engine

- They had ALU's (Arithmetic logic unit) control flow and memory



### Algorithm analysis

- The amount of resources used by the algorithm
    - Space
    - Computational time

- Running time
    - Te number of primitive operations executed before termination

- Order of growth
    - The leading term of the formula 
    - Express behavior as functions approach infinity


### Exponents and Radicals

x^m * x^n = x^m+n

(x^m)^n = x^mn

(xy)^n = x^n y^n

x^1/n = nsqrtx

nsqrtxy = nsqrtx nsqrty

x^m / x^n = x^m-n

x^-n = 1 / x^n

(x/y)^n = x^n / y^n

x^m/n = nsqrtx^m

nsqrt(x/y) = nsqrtx / nsqrty


### Logarithms

- In analysis of algorithms e often use the notation logn without specifying the base
loga x = y means x = a^y

loga 1 = 0

log^k n = (logn)^k

loglogn = log(logn)

logx^y = ylogx

logxy = logx + logy

logx/y = logx - logy

loga x = loga b * logb x

a^logb x = x^logb a

lgn = log2 n

lnn = loge n



### Asymptotic notations
- For each of the following pairs of functions f(n) is either O(g(n)) or theta(g(n)) or omega(g(n))

- Remember theta means equal, o means less than or equal and omega means greater than or equal

- When we say equal we think of it as taking the same time

- When we say greater we think of it taking more time

- When we say less we think of it taking less time

f(n) = logn^2; g(n) = log n + 5. f(n) = theta(g(n)) because they take around the same time

f(n) = n; g(n) = logn^2. f(n) = omega(g(n)) because n is linear and takes longer then log

f(n) = log logn; g(n) = logn. f(n) = o(g(n)) because two logs will make the value smaller, and the algorithm faster

f(n) = n; g(n) = log^2 n. f(n) = omega(g(n)) because n is much slower than log^2n

f(n) = nlogn + n; g(n) = logn. f(n) = omega(g(n)) because nlogn will always be larger, and take more time than logn

f(n) = 10; g(n) = log10. f(n) = theta(g(n)), this is a trick question, they are both constant and therefore take the same time 

f(n) = 2^n; g(n) = 10n^2. f(n) = omega(g(n)) because as n gets higher f(n) will be much larger and take more time

f(n) = 2^n; g(n) = 3^n. f(n) = o(g(n)). because g(n) has a higher base it will take longer



### Asymptotic notation

- O Notation
    - O(g(n)) = {f(n) : there exist positive constants c and n0 such that 0 <= f(n) <= cg(n) for all n >= n0}

- Intuitively O(g(n)) equals the set of functions with a smaller or same order of growth as g(n)