# Week 1-3
## Computer Systems
- __Program__
  * A computer program is a __set of instructions__ for a _computer_ to follow
- __Software__
  * Is the collection of _programs_ by a computer, indcluding:
    + __Editors__
    + __Translators__; and
    + __System Managers__
- __Hardware__
  * It pertains to the __physical parts__ of the _computer system_.
  * The three main classes of computers include:
    + __Personal Computers__ (_PCs_)
      - Relatively small. 
      - Mainly used by one person at a time.
    + __Workstations__
      - Larger and more powerful than a PC.
    + __Mainframes__
      - Still Larger, requires support staff.
      - Shared by multiple users.
- __Computer Organization__
  * Has five main components, namely:
    + __Input Devices__
      - Allows communication on __to the computer__.
    + __Output Devices__
      - Allows communication on __to the user__.
    + __Processor__
      - examples: _CPUs_, _GPUs_, _NPUs_, etc.
      - The CPU can follow _machine langugae_.
    + __Main Memory__
      - Memory locations __containing__ the _running program_, usually stored in a volatile memory called _RAM_.
      - Stores a long list of memory locations, each containing ones and zeros and can change during program execution.
      - Uses a Binary Digit, or a _Bit_, where a digit can only be a one or zero. Each memory location has eight bits.
      - The location in memory is called a _Memory Address_, where it's a series of numbers that identifies a memory location.
      - Accessing memory is done via _Random Access_, hence called _Random Access Memory_ or _RAM_.
    + __Secondary Memory__
      - Its a permanent record of data of on a disk. 
      - Stores instructions between sessions, e.g. a file stores data or instruction in secondary memory.
## __Programming Languages__
- Generations of Programming Languages
  * __Machine Language__
    + First Generation; Composed of binary digits, or ones and zeroes.
    + e.g. 0110 1001 1010 1011
    + The only language that computers understand.
  * __Assembly Language__
    + Second Generation; One-to-one correspondence to machine language, _mnemonic_ rather than binary digits.
    + e.g. MOV rax, 60
  * __Procedural Languages__
    + Third Generation; One instruction translates into many machine language instructions.
    + Closer to natural language; uses common words rather than abbreviated mnemonic, as programs describes the computer's processing step-by-step.
    + e.g. C, C++, Java, Rust, etc.
  * __Non-procedural Langauges__
    + Fourth Generation; Allows the user to specify the desired result without having to specify the detailed procedures needed for achieving the result.
    + e.g. a database query language — SQL
    + Can be used by non-technical users.
  * __Natural Language Programming Languages__
    + Fifth Generation; Intelligent languages; Able to translate natural langauges into a structured, machine-readable form.
    + Are extremely complex and experimental.
- Current Programming Langauges
  * __Object-Oriented Programming__ (_OOP_) Languages
    + Based on _Classes_ and _Objects_; packaging data and the instructions about what to do with that data together.
    + e.g. Java, C++
  * __Visual Programming Languages__
    + Used with a graphical environment, popular to non-technical users.
    + e.g. Visual Basic, Visual C++
  * __Hypertext Markup Langauge__ (_HTML_)
    + Standard language used in World Wide Web (_WWW_).
    + Contains text, images, and other types of information such as data files, audio, video and executable computer programs.
  * __Extensible Markup Language__ (_XML_)
    + Improved on Web document functioncality.
  * __Virtual Reality Modeling Language__ (_VRML_)
    + A file format for describing three-dimensional (_3D_) interactive world and objects, can be used with the World Wide Web.
- Categories of Programming Languages
  * __Procedural Programming__
    + Follows a sequence of statements or commands in order to achieve a desired output.
    + Each series of steps is called a procedure, a program written in one of this langauges will have one or mor procedures within it.
    - e.g. C, C++, Java, Pascal
  * __Functional Programming__
    + Rather than focusing on the execution of statements, functional languages focus on the output of mathematical functions and evaluations.
    + Each function performs a specific task and returns a result — varying on the input data.
    + e.g. Scala, Erlang, Haskell
  * __Object-Oriented Programming__
    + Treats a program as a group of objects composed of data and program elements, also known as attributes and methods.
    + Objects are able to be reused within a program or in other programs, making it popular for complex programs — as code is easier to reuse and scale.
    + e.g. Java, Python, C++
  * __Scripting__
    + Used to automate repetitive tasks, manage dynamic web content, or support processes in larger applications.
    + e.g. Bash, Python, Node.js
  * __Logic Programming__
    + Instead of telling a computer what to do, this type of programming expresses a series of facts and rules to instruct the computer on how to make decisions.
    + e.g. Prolog, Absys, Datalog
* Concepts
  * __Assemblers__
    + A program that translates an assembly source file into machine language.
    + e.g. NASM, MASM, GAS, TASM
  * __Compilers__
    + a program that translates the entire program at once translating high-level langauage to machine language.
    + _Source Code_
      - The original program in a high-level langauge.
    + _Object Code_
      - The translated version in machine language.
  * __Interpreters__
    + a program that translates and executes one source program statement at a time.
    + e.g. Python, JavaScript, Ruby
  * __Linkers__
    + Some programs that are used are already compiled.
      - Their object code if available to be used.
      - e.g. Input and Output routines
    + A linker combines;
      - The object code for the programs that are written, and
      - The object code for the pre-compiled routines into
      - The machine language program that the CPU can run.
## Program Development Life Cycle
- Definition
  * A procedure used in software engineering to control the creation of software programs is called the Program Development Life Cycle (_PDLC_).
  * Used at a higher level to oversee the development of several software projects or programs.
  * It is related to the Software Development Life Cycle (SDLC).
- Program Development
  * Application software is what is used to create application programs — program development, for example.
  * Program development often happens during the system development phase, the SDLC's aquisition phase, and employs to system requirements created duing he system development throughout the SDLC's design phase.
  * The stages of developing a program are referred to as the cycle of program development.
- Program Analysis
  * It is during this stage of the PDLC that the Problem and program requirements are carefully evaluated are created.
  * Class diagrams, input and output deigns, data flow diagrams, database architectures, data dictionaries, and similar requirements are employed in the problem analysis tage of the PDLC.
  * A set of requirements are created by the system analyst during the SDLC's design phase, which describes the new and how the system ought to function.
- Program Design
  * It is during this stage of the PDLC that the program requirements are broadeneed to provide a full design of a fresh program.
  * The requirements created throughout the problem-solving stage are utilized to create a program's algorithm; specifically, the collection of measures that must be taken for the program to carry out all of the things that are expected of it to do.
  * Program Design Tools:
    + Hierarchy Charts
      - Often known as the structure charts — shows how a system is generally structured, a well-defined program.
      - The modules utilized are displayed, in a course and the connections between the modules to another.
    + Flowcharts
      - Are used to show the sequential logic that will be used by a software, a procedure, or a module.
    + Wireframes
      - A visual depiction of an application's general architecture and logic of a website or an app.
    + Pseudocode
      - employs phrases that resemble the English language instead of the graphical symbols seen in flowcharts.
    + Unified Modeling Language (UML)
      - A set of standardized models; A popular tool for developing object-oriented business models programs.
- Program Coding
  * The stage of the SDLC where the program code is created using a programming language to be written.
  * Each programming languages has certain specific syntax to follow, or guidelines, or how to, etc.
  * Certain programming languages may be chose because programs can be written, usually the initial action
  * This stage in PDLC is where a progam is made sure to be accurate and functions properly. Debugging, is the process of making sure that a program is free of errors — where it all begins, the defects or the errors. It is often a time-consuming procedure that can take up a significant amount of time spent creating a program.
- Algorithms, Pseudocodes, and Flowcharts
  * Algorithms
    + Is a precise, step-by-step procedure for solving a problem or accomplishing a task — a fundamental concept in Computer Science and Engineering, serving as the backbone for software development and problem-solving in various fields.
    + It is a finite sequence of well-defined computational steps that transforms input into the desired output, being expressed in various forms — mainly pseudocode and flowcharts.
    + Example Algorithm:
    ```
        Step 1: Start
        Step 2: Read values a and b
        Step 3: Add a and b, assigning the result to sum.
                sum = a + b
        Step 4: Display sum
        Step 5: Stop
    ```
  * Pseudocode
    + Is a text-based method for describing using a combination of natual language and simplified programming constructs.
    + It serves as an intermediate step between human language and actual code, allowing developers to outline the logic and structure of an algorithm without adhering to the strict syntax of a particular programming language.
    + Pseudocode typically includes common programming elements such as loops, conditionals, function calls, but expresses them in a more readable language-agnostic manner.
    + This approach is particularly useful for planning and communicating algorithm designs among a collaboration, as it focuses on the code logic without getting bogged down in implementation details.
    + Example Pseudocode:
    ```
        PRINT "Enter first number: "
        INPUT a
        PRINT "Enter second number: "
        INPUT b
        sum = a + b
        PRINT "Sum =: ", sum
    ```
  * Flowcharts
    + Is a visual representation of an algorithm, using standerdized symbols to depict different types of operations.
    + While algorithms are powerful problem-solving toolsm their textual descriptions can sometimes be challenging to follow, this is where flowcharts comes in to simplify the process.
    + Key Advantages:
      - Visual Clarity
        * They provide a clear, easy-to-understand overview of the process.
      - Improved Communication
        * Facilitates better understanding when collaborating.
      - Identification of bottlenecks
        * Visual representation helps in spotting inefficiencies
      - Documentation
        * Flowcharts serve as excellent tools for process documentation.
    + Example Flowchart:
    ``` mermaid
        flowchart LR
          A([Start]) --> B[/Input two numbers, a and b/]
          B --> C[sum = a + b]
          C --> D[/Print sum/]
          D --> E([Stop])
    ```
    + Symbols and Meanings:
      - Terminal
        * Represents the start or end of a process.
        ``` mermaid
            flowchart 
            A([Oval])
        ```
      - Processing
        * Indicates a processing step or action. A boc where a specific operation or set of operations is performed.
        ``` mermaid
            flowchart LR
            A[Rectnagle]
        ```
      - Input or Output
        * Represents input or output operations. Used for entering data or displaying results.
        ``` mermaid
            flowchart LR
            A[/Parallelogram/]
        ```
      - Decision
        * Shows a decision point in the process. Typically contains a question that can be answered with Yes or no, or True or False.
        ``` mermaid
            flowchart LR
            A{Diamond}
        ```
      - On-page Connector
        * Links one part of the flowchart to another
        ``` mermaid
            flowchart LR
            A((Circle))
        ```
      - Off-page Connector
        * Connects separate parts of a flowchart, used when the flowchart continues on another page.
        ``` mermaid
            flowchart LR
            A>Ribbon]
        ```
      - Flow lines
        * Connects symbols and flow process direction.
        ``` mermaid
            flowchart LR
            A(from) --> B(to)
        ```
      - Preparation
        * Indicates a FOR loop.
        ``` mermaid
            flowchart LR
            A{{Hexagon}}
        ```
      