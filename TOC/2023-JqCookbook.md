# jq Cookbook

<!--- 652 x 841 -->
<img src="https://www.cutt.co.jp/book/images/978-4-87783-508-8.png" width="300">

Satoshi Toyosawa  
Cutt Systems, Tokyo, Japan. 2023.

Japanese edtion is available from
[honto](https://honto.jp/netstore/pd-book_32427461.html),
and other bookstores.


## Table of Contents

Equivalent Python methods are shown in fixed fonts.

- Introduction
- Chatper 1: Number functions
	- N01 Get π
	- N02 Get e (Euler's number)
	- N03 Convert radians to degrees - `math.degfees()`
	- N04 Convert degrees to radians - `math.radians()`
	- N05 Get absolute value - `abs()`
	- N06 Getthe number of bits from integer numbers - `int.bit_length()`
	- N07 Convert digits (base 10) to base N numbers
	- N08 Convert digits (base 10) to binaries (base 2) - `bin()`
	- N09 Convert digits (base 10) to hexadecimas (base 16) - `hex()`
	- N10 Convert base 10 digits to hexadecimals - `hex()`
	- N11 Convert base N numbers to digits - `int()`
	- N12 Convert booleans to numbers
	- N13 Convert empty values to `null`s
	- N14 Return `true` if integers
	- N15 Remove commas from string numbers
	- N16 Insert commans to numbers
	- N17 Extract all numbers in JSON blob
	- N18 Extract all elements of the specific type
	- N19 Round floating point numbers at the specified spots - `f''`string
	- N20 Convert Unix Epock to ISO 8601 format - `datetime.fromtimestamp()`
- Chapter 2: String functions
	- S01 Get Unicode codepoint from strings - `ord()`
	- S02 Get strings from Unicode codepoints - `chr()`
	- S02 Convert numbers to strings - `str()`
	- S04 Captialize strings - `str.capitalize()`
	- S05 Title-case strings - `str.title()`
	- S06 Reverse strings - `reversed()`
	- S07 Swap string cases - `str.swapcase()`
	- S08 Left-justify strings - `str.ljust()`
	- S09 Right-justify strings - `str.rjust()`
	- S10 Justify strings: Select by the argument
	- S11 Center string - `str.center()`
	- S12 Remove whitespaces from the left - `str.lstrip()`
	- S13 Remove whitespaces from the right - `str.rstip()`
	- S14 Remove whitespaces from both left and right - `str.strip()`
	- S15 Convert US dates - `datetime.strftime('%m %d, %Y')`
	- S16 Convert UK dates - `datetime.strftime('%d %m %Y')`
	- S17 Convert syslog timestamps
	- S18 Convert email (RFC 5322) dates
	- S19 Convert version strings to objects
	- S20 Test if the string is IPv4 address
	- S21 Test if the string is MAC address
	- S22 Convert HTTP response headers to objects
	- S23 Colorize strings
	- S24 Parse the `JQ_COLORS` environment variables
	- S25 Convert alphabets from full-width to normal ASCIIs.
- Chapter 3: Array functions
	- A01 Square element-wise - `numpy.square()`
	- A02 Add element-wise - `numpy.add()`
	- A03 Return the dot products - `numpy.dot()`
	- A04 Return the cross products - `numpy.cross()`
	- A05 Calculate the distances - `math.dist()`
	- A06 Generate the Cartesian product - `itertools.product()`
	- A07 Generate an array of alphabets
	- A08 Insert an array to another array - `list.extend()`
	- A09 Split arrays
	- A10 Slice with steps - `list[start:end:step]`
	- A11 Count the number of elements - `list.count()`
	- A12 Find the longest character length in the nested arrays
	- A13 Sort case-insensitively
	- A14 Convert array of arrays to table format
	- A15 Convert text file to array of arrays
	- A16 Convert CSV file to array of arrays
	- A17 Objectify arrays
	- A18 Objectify two arrays (1st array is the keys, 2nd is the values)
	- A19 Output the searched element along with the traling or preceding elements
- Chapter 4: Set function
	- M01 Create sets - `set()`
	- M02 Add element to the set - `set.add()`
	- M03 Remove elements from the set - `set.remove()`
	- M04 Calculate union - `set.union()`
	- M05 Calculate intersection - `set.intersection()`
	- M06 Caclulate difference - `set.differnece()`
	- M07 Calculate symmetric_difference - `set.symmetric_difference()`
	- M08 Test if subset - `set.issubset()`
	- M09 Test if superset - `set.issuperset()`
	- M10 Test if disjoint - `set.isdisjoint()`
- Chapter 5: Statistical functions
	- E01 Sum - `sum()`
	- E02 Mean - `statistics.mean()`
	- E03 Median - `statics.median()`
	- E04 Mode - `statics.mode()`
	- E05 Population variance - `statistics.pvariance()`
	- E06 Population standard deviation - `statistics.pstdev()`
	- E07 Sample variance - `statistics.variance()`
	- E08 Sample standard deviation - `statistics.stdev()`
- Chapter 6: Object functions
	- O01 Recursively extract property keys
	- O02 Extract both keys and values
	- O03 Swap property keys and values
	- O04 Create object using one of the values as the key
	- O05 Create arrays from objects
	- O06 Extract objects without the specific keys
	- O07 Add properties if not present
	- O08 Find the missing properties
	- O09 Sort by property key length
	- O10 Sort by property key in nested objects
	- O11 Multiply property values
	- O12 Convert objects to CSV
	- O13 Convert CSV file to object
- Chapter 7: SQL functions
	- Q01 `SELECT * FROM table;`
	- Q02 `SELECT * FROM table ORDER BY column;`
	- Q03 `SELECT * FROM table ORDER BY column DESC;`
	- Q04 `SELECT columns FROM table;`
	- Q05 `SELECT column * num FROM table;`
	- Q06 `SELECT * FROM table WHERE column = value;`
	- Q07 `SELECT * FROM table WHERE column IN (values);`
	- Q08 `SELECT * FROM table WHERE column BETWEEN num1 AND num2;`
	- Q09 `SELECT COUNT(*) FROM table;`
	- Q10 `SELECT * FROM table1 UNION ALL SELECT * FROM table2;`
	- Q11 `SELECT * FROM table1 INTERSECT SELECT * FROM table2;`
	- Q12 `SELECT * FROM table1 INNER JOIN table2 ON table1.column = table2.column;`
	- Q13 `DESC table;`
	- Q14 `INSERT INTO table VALUES(values);`
	- Q15 `UPDATE table SET column1 = value1 WHERE column2 = value2;`
	- Q16 `DELETE FROM table WHERE column = value;`
	- Q17 `ALTER TABLE table DROP COLUMN column;`
	- Q18 `ALTER TABLE table ADD COLUMN column DEFAULT value`
	- Q19 `DROP table;`
 - Chatper 8: Algorithm functions
	- F01 Multiplication table
	- F02 Factorial (loop)
	- F03 Factorial (recursion)
	- F04 Fibonacci series (loop)
	- F05 Fibonacci series (recursion)
	- F06 Primes
	- F07 π 
	- F08 e
- Chapter 9: Miscellaneous functions
	- T01 Ignore non-JSON inputs
	- T02 Process by line numbers
	- T03 Use environment variable for specifying properties
	- T04 Convert objects to environment variables
	- T05 Specify properties from the command line argument
	- T06 Read the paths from a file and extract
- Appendix A: Defining functions
- Appendix B: Built-in function hints
- Appendix C: Terminology
- Appendix D: Special characters
- Appnedix E: List of the functions in this book
 