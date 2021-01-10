1. Read the problem
2. Make sure that you understand the problem
   - Do you understand all the terms used?
   - Can you restate the problem in your own words?
   - Do you understand all the limitations? Which parameters are integers and which are reals? Are some numbers strictly positive? How large are arrays? How long can be strings? If you program with C++ do some numbers overflow int? etc.
   - Can you think of at least one input and expected output?
3. Create a test set of at least two inputs and expected outputs, make sure that you understand all corner cases.
4. Think about solution in general, suppose that someone will provide you with a "magic library" that has all standard algorithms (e.g. quicksort) implemented. Sketch your solution.
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
