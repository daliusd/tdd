## The Three Rules of TDD

1. You are not allowed to write any production code unless it is to make a failing unit test pass.
2. You are not allowed to write any more of a unit test than is sufficient to fail; and compilation failures are failures.
3. You are not allowed to write any more production code than is sufficient to pass the one failing unit test.

Which means the workflow is:

1. Write a failing test. Stop writing the test as soon as it fails.
2. Write the minimal production code required for the test to pass. Stop writing any code once the test passes.
3. Refactor the test code and the production code without altering the functionality. All tests should pass.

## Usage
To run the tests, run `npm run test`.

## String Calculator
Made popular by [Roy Osherove](http://osherove.com/tdd-kata-1/).

#### Before you start:
* **Try not to read ahead.**
* **Do one task at a time. The trick is to learn to work incrementally.**
* **Make sure you only test for correct inputs. there is no need to test for invalid inputs for this kata**

This kata is one of the simplest and best ways to practice step-by-step fluent tdd, and provides an easy way to get proficient in a language.

Write a method `add` under an object `StringCalculator` that, given a delimited string, returns the sum of the numbers in the string.

1. An empty string returns zero `'' => 0`
2. A single number returns the value `'1' => 1` `'2' => 2`
3. Two numbers, comma delimited, returns the sum `'1,2' => 3` `'10,20' => 30`
4. Two numbers, newline delimited, returns the sum `'1\n2' => 3`
5. Three numbers, delimited either way, returns the sum `'1\n2,3\n4' => 10`
6. Negative numbers throw an exception with the message `'-1,2,-3' => 'negatives not allowed: -1,-3'`

**stop here if you are a beginner. Continue if you can finish the steps so far in less than 30 minutes.**

7. Numbers greater than 1000 are ignored
8. A single char delimiter can be defined on the first line starting with `//` (e.g `//#\n1#2` for a ‘#’ as the delimiter)
9. A multi char delimiter can be defined on the first line starting with `//` (e.g. `//###\n1###2` for ‘###’ as the delimiter)
