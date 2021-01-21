# How to approach the problem

1. Read the problem
2. Make sure that you understand the problem
   - Do you understand all the terms used?
   - Can you restate the problem in your own words?
   - Do you understand all the limitations? Which parameters are integers and which are reals? Are some numbers strictly positive? How large are arrays? How long can be strings? If you program with C++ do some numbers overflow int? etc.
   - Can you think of at least one input and expected output?
   - Draw the picture if that is possible.
3. Create a test set of at least two inputs and expected outputs, make sure that you understand all corner cases. Draw the picture if that is possible.
4. Think about solution in general, suppose that someone will provide you with a "magic library" that has all standard algorithms (e.g. quicksort) implemented. Sketch your solution. If no idea comes to your mind, see the next section.
5. Try your solution on your testcases. Fix problems if they appear. If you spotted a fundamental flaw that cannot be fixed return to 4.
6. Check complexities
   - Estimate complexity of your solution.
   - Estimate the lower bound complexity of any possible solution (e.g. if changing one of the array's elements changes the entire result, you should look at each element at least once, thus no better solution than O(n)). 
   - How strongly do your complexities disagree? If the disagreement is very strong, rethink your lower bound estimate first and return to 4 if nothing changes. (if you have no time, proceed with your solution as is -- it is better to create bad solution than no solution)
7. Implement
   - Write the main function, use standard algorithms as if they were implemented for you in some "magic library"
   - Check which unimplemented functions did you use, implement them. Don't forget to check them with custom inputs and expected outputs.
   - Check the whole algorithm against your custom inputs.
8. Debug
   - Check corner cases, fix problems if they appear.
   - Think of at least one more input and expected output you didn't use previously, fix problems if they appear.
9. If you have some more time -- optimize.

# I'm running out of ideas, what to do?

Basically, there is no general approach to solve any problem (obviously), but I tried to collect all the techniques that come to my mind and can be useful.

1. Remember all similar problems, they may give you a hint which way to look for the solution.
2. Simplify the problem -- its simpler version may give you some insights into the original problem
   * Perform simplification
       - if the problem considers many dimensions, try reducing them to 1 or 2
       - if the problem considers many elements, try solving the same for 2 or 3 elements
       - etc
   * Solve the simplified version
   * Return to the original problem
       - can you solve the original problem now?
       - check if original problem can be reduced to the simplified version by some procedure
       - check if original problem is equivalent to the simplified version (maybe, you'll need to prove some statements)
3. Mathematical induction approach
   - Suppose, you have a function that solves the problem for N elements, can you solve it for N+1 ?
   - Suppose, you have a function that solves the problem for N elements, can you solve it for 2*N ?
4. Split the problem
   - Can you represent the problem as few subproblems and solve them separately?
   - Are there any additional data that may help you?
   - Can you solve the problem if you have these data?
   - Can it be more easy to focus on obtaining these data instead of the original problem?
5. Special cases
   - Are there any restrictions that may help you to solve the problem?
   - Apply these restrictions and solve the problem.
   - Can you think on how to solve the problem without restrictions?
   - Can you find a method of reducing the original problem to the restricted problem?
6. One particular case
   - Can you solve the problem "by hands" for one certain input?
   - Can you somehow transform your solution to something comprehensible by computer?
