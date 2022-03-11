## Lab Report 4 Week 8
---


**Finding Different Results**

To find different outputs, I simply used `diff` on the resuls.txt file for the two different implementations. A section of the output of the `diff` command is pictured below.

![Image](diff.png)

**Difference Test 12**

The difference on line 47 corresponds to test 12, which is the following md file:

![Image](test1.png)

My implementation returns [\\] while the other implementation returns [], which is the correct answer. The reason my implementation returns [\\] is because it doesn't properly check that there are corresponding parentheses for the brackets. I did include a check, but it searches for open parentheses after the current index and not the index of the brackets. To fix this, I should either change the starting index to search for open parentheses to nextCloseBracket or add a separate check for directly after the bracket.

![Image](fix1.png)

> [Foo*bar\]]:my_(url) 'title (with parens)'

[Foo*bar\]]