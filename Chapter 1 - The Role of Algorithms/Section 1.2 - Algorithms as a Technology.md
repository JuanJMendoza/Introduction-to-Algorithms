## Section 1.2: Algorithms as a Technology
### Exercises

#### 1.2-1
Give an example of an application that requires algorithmic content at the application level, and discuss the function of the algorithms involved.

***Answer:*** Google maps is an application that requires algorithmic content at the application level because it gathers all the possible routes one can take to get from point A to point B using graph algorithms and does so respective to the mode of transportation we choose to take to get there. i.e., by transit, driving, etc.


#### 1.2-2
Suppose we are comparing implementations of insertion sort and merge sort on the same machine. For inputs of size n, insertion sort runs in 8n^2 steps, while merge sort runs in 64n lg n steps. For which values of n does insertion sort beat merge sort?

***Answer:*** To figure out the values of n for which insertion sort beats merge sort we have to solve the inequality of 8n² < 64nlog(n)  which after some algebra evaluates to 2^(n/8) < n. From here, we figure the values in which insertion sort (2^(n/8)) beats out merge sort (n). Since we know merge sort beats out insertion sort when n = 1, we will start from n = 2. If we use any integer between 2 and 8 we will get a decimial so we will work with powers of 2. When n = 8 the inequalites for insertion sort and merge sort evaluate to 2 < 8, respectively. We try n = 64, which evaluates to 256 < 64, it seems we passed the upper boundary of which merge sort began to beat insertion sort again. We begin to use binary search to find the lower and upper bounders by finding the mean of the current lower and upper boundaries (lower + upper) / 2). After some iterations we come up with n = 43, which evaluates to 41.49 < 43. If we use n = 44, the inequality evaluates to 44.8 > 44. From the last two shown expressions, its clear for values 2 <= n <= 43 insertion sort beats out mergesort.

#### 1.2-3
What is the smallest value of n such that an algorithm whose running time is 100n2 runs faster than an algorithm whose running time is 2ⁿ on the same machine?

***Answer:*** An algorithm which runs at 100n² (Algorithm A) will run faster than one with a runtime of 2ⁿ (Algorithm B) for a large enough n. To find the smallest value for which A begins to run faster than B we will pass in values which will be powers of 2 to n. For n = 2 A < B evaluates to 400 < 4, next we try the next power of 2, which is 4 and has A < B evaluate to 1600 < 16. We continue this until we get to n = 16 where the inequality A < B evalutes to 25,600 < 65,536. We do what we did above and find the mean of the upper and lower bounds. We get n = 15 which is the smalled number in which the A < B is true.

