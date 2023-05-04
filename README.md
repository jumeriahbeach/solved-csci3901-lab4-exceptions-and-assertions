Download Link: https://assignmentchef.com/product/solved-csci3901-lab4-exceptions-and-assertions
<br>
In this lab, you will practice using exceptions and assertions.

you will create two small programs that demonstrate how to use exceptions and assertions.

<h1>Preparation</h1>

<ul>

 <li>Review the discussion on exceptions from class.</li>

 <li>Review the recursive code for calculating the <strong>Fibonacci </strong>numbers from the debugging lab.</li>

 <li>Prepare pseudocode to implement a non-recursive <strong>binary search </strong>on an array of integers.</li>

</ul>

<h1>Procedure</h1>

<strong>Set-up</strong>

<ol>

 <li>Get the recursive code for calculating the Fibonacci numbers working in a project.</li>

</ol>

<strong>Lab steps</strong>

<h2>Part 1 – Exceptions</h2>

<ol>

 <li>Revise the Fibonacci code as follows to be able to limit the depth of the recursion:

  <ul>

   <li>Add two parameters to the method: one to say the maximum number of levels of recursion should be allowed and the second to say how deep you are now in the recursion</li>

   <li>When the code calls itself recursively, increment the parameter on how deep you are into the recursion</li>

  </ul></li>

 <li>Create a custom-made exception called MaximumRecursionDepth that extends the RuntimeException The new exception should include a String message and an int that is the depth of recursion reached. Ensure that your custom-made exception has two methods available:

  <ul>

   <li>getMessage() to return the string message</li>

   <li>getDepth() to return the integer depth that was reached at the time of the exception</li>

  </ul></li>

 <li>Modify your Fibonacci code to throw a MaximumRecursionDepth exception when the recursion depth exceeds the value of the parameter for the maximum number of levels of recursion.</li>

</ol>

1

<h2>Part 2 – Assertions</h2>

<ol>

 <li>Write (non-recursive) code to perform a binary search on a sorted array. You can get help from the Internet for this part; just be sure to cite any sources that you use. This step is not the critical one of the lab.</li>

 <li>Add the following assertions:

  <ul>

   <li>a loop precondition</li>

   <li>a loop invariant</li>

   <li>a postcondition</li>

  </ul></li>

 <li>Ensure that your assertions are working.</li>

</ol>

<h1>Questions</h1>

We usually want you to re-use existing code and infrastructure whenever possible. Why might you create your own exception?

We added parameters to the Fibonacci method. However, those parameters aren’t very meaningful to a general user. What would you do to the code to make it more accessible for a general user?

How would you recommend for someone to develop a loop invariant?

How can loop invariants help you in programming, even if you don’t include them directly as assertions in your code?