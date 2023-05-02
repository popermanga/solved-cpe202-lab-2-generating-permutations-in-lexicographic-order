Download Link: https://assignmentchef.com/product/solved-cpe202-lab-2-generating-permutations-in-lexicographic-order
<br>
Goal: Write a Python program to generate all the permutations of the characters in a string.  This will give you a chance to  review some simple Python constructs, i.e.. Strings and Lists and solidify your understanding of recursion.

Your program <strong><u>must</u></strong> meet the following specification. You are to write a Python function <strong>perm_lex </strong>that:

<ul>

 <li>Takes a string as a single input argument. You may assume the string consists of <strong>distinct lower case</strong> letters (in alphabetical order).  You may assume the input is a string of letters <u>in alphabetical order</u>.</li>

 <li>Returns is a <strong><u>list</u></strong> of strings where each string represents a permutation of the input string. The list of permutations must be in lexicographic order. (This is basically the ordering that dictionaries use.  Order by the first letter (alphabetically), if tie then use the second letter, etc.</li>

 <li>You need to use <strong>design recipe</strong> for this lab assignment. I will offer you the step 4, which is template and you need to cover all other steps.</li>

 <li><strong>NOTE</strong>: You only allow to use basic library functions of Python! If the string is empty return empty list.</li>

</ul>

<strong>Argument:</strong>     abc

<strong>Returns:      </strong>[abc, acb, bac, bca, cab, cba]

Step 4: Templet (Pseudocode for a recursive algorithm to generate permutations in lexicographic order.) <strong>You must follow this pseudo code. </strong>

<ul>

 <li>If the string contains a single character return a list containing that string</li>

 <li>Loop through all character positions of the string containing the characters to be permuted, for each character:

  <ul>

   <li>Form a simpler string by removing the character o Generate all permutations of the simpler string recursively</li>

   <li>Add the removed character to the front of each permutation of the simpler word, and</li>

   <li>add the resulting permutation to a list</li>

  </ul></li>

 <li>Return all these newly constructed permutations</li>

</ul>

Submit you Python function in a file called <strong>perm_lex.py</strong> to Polylearn and your test program in <strong>perm_lex_testcases.py. Do not submit your files as zip file and use exactly the same file names and function name. </strong>

Note:  For a string with n characters, you program will return a list contain n! strings.  Note that n! grows very quickly.  For example : 15! is roughly 1.3*10<sup>12</sup> .  Thus it is probably not a good idea to test your program with long strings.

Your test cases must cover all possible situations.