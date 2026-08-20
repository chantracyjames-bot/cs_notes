### > [Table of Contents](../main.md)
# CC104
---
## Problem Solving Process (PSP)
- Background
	- Programs are comprised of:
		* Data; and
		* Algorithms
	- __Programming__ is a problem solving process, wherein;
		* the problem is defined,
		* the data to manipulate and work on is distinguished, and
		* the expected result is determined.
	- It is implemented in a machine known as a _computer_ and the operations provided by the machine is used to solve the given problem.
- Definition
	- It could be viewed in the following terms of domains; problem, machine, and solution.
* __Problem Domain__
   + According to C2 Wiki:
		- The Problem Domain is a term that refers to all information that defines the problem and constrains the solution, the constraints being part of the problem.
		- It includes the goals of the author of the problem wished to achieve, the context (and setting) within which the problem exists in, and all rules taht define essential functions or other aspects of any solution product.
		- It represents the environment in which a solution will have to operate in, as well as the problem itself.
		- Keep in mind that the customer for a software solution, the "author" of the problem, doesn't necessarily recognise the existence of a problem so much as an opportunity.
		- An engineer sees the "problem domain" as being the set of circumstances for which they have to provide a solution.
		- Meaning; It's the engineer's problem, not the customer's.
	+ It includes the _input_, or the _raw data_ to process, and the _output_, or the _processed data_.
	+ Example:
		- In sorting a set of numbers, the raw data is the set of numbers in the original order and the process data is the numbers in a sorted order.
      > | Raw Data       | Processed Data         |
       > | -------------- | ---------------------- |
       > | Personal Data  | Academic Histories     |
       > | Form 5s        | Performance Indicators |
       > | Grading Sheets | Transcripts            |
       > | etc.           | etc.                   |

* __Machine Domain__
	+ consists of the _storage medium_ and _processing unit_.
	+ __Storage Medium__
		- consists of serially arranged bits that are addresable as a unit.
		- e.g. bits, bytes, words, etc.
	+ __Processing Unit__
		- allows the use of basic operations.
		- inclused arithmetic, comparisons, etc.
	- Example:
      > | Storage Medium | Processing units |
       > |------|------|
       > | Bits | Add, Subtact |
       > | Bytes | Multiply |
       > | Words | Divide |
       > | etc. | etc. |

* __Solution Domain__
	+ **links the _problem_ and _machine_ domains**.
	+ It is at the solution domain where structuring of higher level _data structures_ and synthesis of _algorithms_ are of concern.
	+ Example:
      > | Data Representations | Algorithms |
       > |---|---|
       > | Lists | Searching |
       > | Files | Sorting | 
       > | Tables | Memory Management |
       > | Trees | Traversal |
       > | etc. | etc. |
## Algorithms
- Definition:
	* The term algorithm is used in computer science to describe a _finite_, _deterministic_, and effective _problem solving method_ suitable for implementation as a computer program.
	* It is __strictly defined__ _finite sequence_ of well-defined statements that provides the __solution__ to a problem for any acceptable set of input values (if there are any).
	* The term _finite_ means that the algorithm should __reach an end point__ and __cannnot run indefinitely__.
- Function:
	* An algorithm is a _step-by-step procedure_.
	* Which defines a _set of instructions_ to be executed in a _certain order_ to get the desired output.
	* Algorithms are generally created __independent of any underlying languages__, i.e. an algorthm can be implemented in __more than one programming language__.
- Example:
	> Making a cup of tea: 
	> 1. Put the teabag in a cup. 
	> 2. Fill a kettle with water. 
	> 3. Boil the water in the kettle. 
	> 4. Pour some of the boild watter into the cup. 
	> 5. Add milk to the cup. 
	> 6. Add sugar to the cup. 
	> 7. Stir the tea in the cup. 
	> 8. The tea is ready.
    
+ Note:
	+ That there are a certain amount of steps that __must be followed__.
	+ These steps are in a _specific order_, even though some of the steps could be rearranged; like steps 5 and 6, which can be reversed without any problems.
	+ Aside from the certain amount of steps that must be performed, the entire process is _finite_ and reaches its end point, allowing the goals to be achieved (in this case, making a cup of tea).
- __Fundamental Properties of Algorithms__
	* __Finiteness__
		+ An algorithm __must terminate__ after a finite number of steps.
	* __Definiteness__
		+ An algorithm must ensure that every step is __precisely defined__.
		+ For example "divide a number by x" is not sufficient. The number x must be defined precisely, say a positive integer.
	* __Input__
		+ The _domain_ of the algorithm which could be zero or more quantities (as input).
		+ Which becomes the pieces of data to work with.
	* __Output__
		+ Set of one or more resulting quantites (results), also called the _range_ of the algorithm.
	* __Effectiveness__
		+ Each step or operations in the algorithm are suffieciently __as basic as they can__.
		* In principle, they can be done exactly and in finite time __by a person using a pen and paper__.
## Mathematical Functions
- Types of Functions
	- __Floor and Ceiling__
		* Floor
			+ Flooring a number means taking the __greatest integer__ that is __less than or equal to__ x, where x is any __real number__.
			+ It uses the _Cartesian Plane_ as a basis, taking the __greatest integer__ that is to the __left__ of x.
			- Example: 
          > | Numbers | Floor |
            > |:---:|:---:|
            > | 3.14 | 3 |
           >  | 1/2 | 0 |
            > | -1/2 | -1 | 
            > | 2.72 | 2 |
            > | -1.2 | -2 |
            > | 1.2 | 1 |
		* Ceiling
			+ Celiing a number means taking the __smallest integer__ that is __greater than or equal to__ x, where x is any __real number__.
			+ It uses the _Cartesian Plane_ as a basis, taking the __smallest integer__ that is to the __right__ of x.
			+ Example:
          > | Number | Ceiling |
            > |---|---|
            > | 3.14 | 4 |
            > | 1/2 | 1 |
            > | -1/2 | 0 |
            > | 1.1 | 2 |
            > | -2.3 | -2 |
            > | 4.19 | 5 |
		- __Modulo__
			* The remainder operation
			+ It is the remainder of a division operation
          > | Expression | Modulo |
            > |---|---|
            > | 9 mod 2 | 1 |
            > | 4 mod 2 | 0 |
            > | 0 mod 3 | 0 |
            > | 1 mod 0 | 0 (undefined) |
- __Identities of Mathematical Functions__
  * $\Large \lceil x \rceil = \lfloor x \rfloor$
    + if and only if __x is an integer__
  * $\Large \lceil x \rceil = \lfloor x \rfloor + 1$
    + if and only if __x is not an integer__
  * $\Large \lfloor -x \rfloor = - \lceil x \rceil$
  * $\Large \lfloor x \rfloor + \lfloor y \rfloor <= \lfloor x + y \rfloor$
  * $\Large x = \lfloor x \rfloor +\ x\ mod\ 1$
  * $\Large z(x\ mod\ y) = zx\ mod\ zy$
# > [Lesson 2](CC104/Lesson%202.md)
<!--
- Advanced Review
    - Basic Operations
        - Addition
            - example:
                1 + 1 = 2
                9 + 10 = 21
        - Subtraction
            - example:
                -1 - -1 = 0
                1 - 1 = 0
        - Multiplication
            - example:
                -1 * -6 = 6
                6 * 2 = 12
        - Division
            - example:
                2 / 2 = 1
                -2 / -1 = 2
    - Absolute Numbers
        - is the distance of the number from zero
        - or the positive sign of a negative number 
            - example:
                -3 = 3
                0 = 0
                2 = 2
    - Laws of Negativity
        - how numbers behave when interacting with negative numbers
        - in Addition
            - when adding two numbers with different signs
                - the sign of the higher absolute value takes precedence
                    - example:
                        1 + -8 = -7
                - if both are the same sign, then the sum inherits the corresponding sign
                    - example:
                        -1 - -3 = -4
        - in Subtraction
            - when subtracting two numbers with the opposite sign
                - change the operation into addition and flip the sign of the second number
                    - example:
                        5 - (-2) = 5 + 2 = 7
                        -7 - -8 = -7 + 8 = 1
        - in Multiplication
            - when multipying two numbers with the opposite sign
                - the product will always be negative
                    - example:
                        -9 * 2 = -18
                - if they both have the same sign, then the product is always positive
                    - example:
                        -3 * -4 = 12
        - in Division
            - when dividing two numbers with the opposite sign
                - the qoutient will always be negative
                    - example:
                        -8 / 4 = -2
                        12 / -3 = -4
                - if both numbers have the same sign, the qoutient will always be positive
                    - example:
                        -8 / -4 = 2
    - Exponents and Logarithms
        - Exponents 
            - is the operation of raising a number to a certain magnitude
                - i.e. multipying the number by itself according to the exponent
            - example:
                6^2 = 36
                3^4 = 81
                4^3 = 64
        - Logarithms 
            - is the operation of finding the exponent (n) of a base number (a)
                - that should result into the value (b)
            - syntax:
                log_a b = n
                // wherein
                    // a is the base number
                    // b is the value after exponentiation
                    // n is the exponent
                // in exponent form
                a^n = b
            - example
                log_2 64 = 6
                // in exponent form
                2^6 = 64
    - Factorials, Combinations and Permutations
        - Factorials
            - multiplies the number by the integers preceding it until zero
                - denoted by the exclamation synbol
            - example:
                4! = 4 * 3 * 2 * 1 = 24
                6! = 6 * 5 * 4 * 3 * 2 * 1 = 720
        - Permutations
            - are the ordered Combinations of objects where sequence and order matters
                - denoted with the formula of:
                    P = (n!) / (n - r)!
            - example:
                where:
                    n = 3
                    r = 2
                P = (3!) / (3 - 2)!
                  = (3 * 2 * 1) / (1)!
                  = 6 / 1
                  = 6
        - Combinations
            - is the way of choosing items from a larger group
                - wherein order does not matters
                - formula:
                    C = (n!) / [(n - r)! * (r!)]
            - example:
                where:
                    n = 3
                    r = 2
                C = (3!) / [(3 - 2)! * (2!)]
                  = (3 * 2 * 1) / [(1)! * (2 * 1)]
                  = 6 / [1 * 2]
                  = 6 / 2
                  = 3
--> 
