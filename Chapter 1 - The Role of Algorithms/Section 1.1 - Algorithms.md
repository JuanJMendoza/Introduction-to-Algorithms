## Section 1.1: Algorithms
### Exercises

#### 1.1-1 
Give a real-world example that requires sorting or a real-world example that requires computing a convex hull.

***Answer:*** A real-world example that would require sorting is when recruiters are trying to figure out who to contact for a job/internship they would sort the candidates/resumes by experience. 


#### 1.1-2
Other than speed, what other measures of efficiency might one use in a real-world setting?

***Answer:*** Other than speed, another measure of efficiency one might use in a real-world setting is space/memory efficency.


#### 1.1-3
Select a data structure that you have seen previously, and discuss its strengths and limitations.

***Answer:*** Arrays have the ability for random-access memory since it's indexed giving it a constant time O(1) 'get' functionality. On the other hand, if we don't know where in the Array an element is, we would have to traverese through the entire array giving it a linear time O(n), where n is the number of elements in the array, look up functionality.


#### 1.1-4
How are the shortest-path and traveling-salesman problems given above similar? How are they different?

***Answer:*** 

**Similarities:** Both the shortest-path and traveling-salesman problems are graph problems that get us from point A to point B.

**Differences:** The shortest-path problem involves getting from point A to point B by traversing through as few edges as possible, potentially leaving out visiting some nodes. As for the traveling-salesman problem, it involves getting to point A to point B by ensuring we go through every other node with each node's next visiting node being its closest neighbor until we inevitably reach point B.


#### 1.1-5
Come up with a real-world problem in which only the best solution will do. Then come up with one in which a solution that is “approximately” the best is good enough.

***Answer:*** 

**Best Solution:** For this scenario, an anesthesiologist has to get the amount of anesthesia they will be giving a patient right or else they risk not giving the patient enough anesthesia to sidate them for their procedure or potentially killing them.

**Approximate Solution:** For a scenario where an approximate is good enough is when someone is cooking and they don't have a measuring utinsil to measure the amount of ingredient they're adding to a dish, they can approximate the amount and be off by a little and still be okay.

