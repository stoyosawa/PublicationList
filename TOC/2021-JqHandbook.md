# jq Handobook

<!--- 652 x 841 -->
<img src="https://www.cutt.co.jp/book/images/978-4-87783-491-3.png" width="300">

Satoshi Toyosawa  
Cutt Systems, Tokyo, Japan. 2021.

Japanese edtion is available from
[amazon.co.jp](https://www.amazon.co.jp/dp/4877834915),
[honto](https://honto.jp/netstore/pd-book_31037910.html),
[Yodobashi](https://www.yodobashi.com/product/100000009003450000/),
and other bookstores.

## Table of Contents

- Introduction
- Chapter 1: Let's Get Started
	- 1.1 Running `jq`
	- 1.2 Filters
	- 1.3 Command options
	- 1.4 Summary
- Chapter 2: Input/Output
	- 2.1 Input
	- 2.2 Filter file
	- 2.3 Exit codes
	- 2.4 Output conversions
	- 2.5 Summary
- Chapter 3: Basic Filters
	- 3.1 Square brackets `[]`
	- 3.2 Comma `,`
	- 3.3 Pipe `|`
	- 3.4 Quesion mark `?`
	- 3.5 Curly brackets `{}`
	- 3.6 Double dots (`..`)
	- 3.7 Summary
- Chapter 4: Basic Operations and JSON Data Types
	- 4.1 Operators and functions
	- 4.2 JSON Data types
	- 4.3 Addition and subtraction
	- 4.4 Type-dependent functions
	- 4.5 Substitution
	- 4.6 Summary
- Chapter 5: Number Operations
	- 5.1 Multiplication and division
	- 5.2 Rounding
	- 5.3 Decomposing numbers
	- 5.4 Math functions
	- 5.5 Generating numerical list
	- 5.6 Date/time functions
	- 5.7 Numeric constants
	- 5.8 IEEE 754 and precisions
	- 5.9 Summary
- Chapter 6: String Operations
	- 6.1 Basic operations
	- 6.2 Regular expression
	- 6.3 Summary
- Chapter 7: Array Operations
	- 7.1 Extracing elements
	- 7.2 Reshaping array
	- 7.3 Sequence operation
	- 7.4 Summary
- Chapter 8: Object Operations
	- 8.1 Basic operations
	- 8.2 Manipulating keys and values
	- 8.3 Path array
	- 8.4 Summary
- Chapter 9: Operators and Predicates
	- 9.1 Comparison operators
	- 9.2 Predicate functions
	- 9.3 Summary
- Chapter 10: Flow Control
	- 10.1 Conditional branching
	- 10.2 Error trapping
	- 10.3 Variables
	- 10.4 Defining function
	- 10.5 Loop
	- 10.6 Summary
- Appendices:
	- Appendix A: Installation
	- Appendix B: JSON data types
	- Appendix C: List of commands
	- Appendix D: References



Sample: Fibonacci function (recursive)

```
$ jq -cn 'def fibonacci_recurse($loop):
    length as $len |
    if $len >= $loop then
        .
    else
        if $len == 0 then
            [0]
        elif $len == 1 then
            [0, 1]
        else
            . + [.[$len-1] + .[$len-2]]
        end |
        fibonacci_recurse($loop)
    end; fibonacci_recurse(30)'
[0,1,1,2,3,5,8,13,21,34,55,89,144,233,377,610,987,1597,2584,4181,6765,10946,
 17711,28657,46368,75025,121393,196418,317811,514229]
```
