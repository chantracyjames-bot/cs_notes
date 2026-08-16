# Topic 1 & 2
## Background
- Relationship between Architecture and Organization
  *__Definition__
    + Architecture
      - The schematics, planning, foundations, structure and interior of a concept.
      - Is the Functional System Design of a computer.
    + Organization
      - The consolidation, interconnection, management, arragement and group.
      - Is the Network of Interconnected Devices.
      - Either through any forms of connectivity, may it be:
        * Wired Connections
        * Wireless Connections

  * __Relationship__
    + The relation between Architecture and Organization is formed through a Symbiotic Relationship. Wherein, the Organization (e.g. peripherals like BUS) is called into use by the Architecture (e.g. the Processor).
      - The Architecture sits inside the computer.
      - The Organization is what is plugged into a computer.
    + Example:
      - When a computer that is formed by the Architecture needs the connected peripherals of the Organization; or
      - When the CPU requests to the motherboard the currently connected USB device.

- CISC vs RISC
  *__CISC__
    + _Complex Instruction Set Computers_
    + It carries out complex instructions.
    + Taking multiple cycles to complete a single instruction.
    + it has the advantage of speed at the cost of complexity (difficulty).

  * __RISC__
    + _Reduced Instruction Set Computers_
    + it carries out simple (reduced) instructions.
    + taking around a single cycle to complete a single instruction
    + it has the advantage of simplified implementation at the cost of slow speed.

## Target
- Learning Outcomes
  * Define computer
  * Define the scope of computer organization and explain its role in the functionality of computer systems.
  * Define the scope of computer architecture and describe its impact on system design and performance. 
  * Identify common goals shared by computer organization and computer architecture and explain their interdependence.
  * Contrast computer organization and computer architecture by highlighting their differences in terms of system functionality, design, and performance. 
  * Define computer organization and explain its significance in the operation of computer systems.
  * Define computer architecture and explain its  ignificance in the design and performance of  computer systems.
  * Distinguish between computer organization and computer architecture by comparing their roles, focus areas, and impact on system functionality.
- Topics
  1. Introduction to Computer Organization and Computer Architecture
    + 1.1. What is Computer, its features, advantages, disadvantages?
    + 1.2. Scope of Computer Organization
    + 1.3. Scope of Computer Architecture
    + 1.4. Common Goals and Interdependence
    + 1.5. Contrast Between Computer Organization 
  2. Computer Organization (CO) VS Computer Architecture (CA)
    + 2.1.Definition and significance.
    + 2.2.Distinction between computer organization and computer architecture.

## What is a Computer?
- Definition
  * A computer is an _electronic device_ that can __process and store information__.
  * It can __perform calculations__, __manipulate data__, and __execute instructions__ to __accomplish specific tasks__.
  * The basic components of a computer includes:
    + Processors — e.g. Central Processing Unit (_CPU_) 
    + Memory — e.g. Random Access Memory (_RAM_),
    + Storage — e.g. Hard Disk Drives or Solid-state Drives (_HDDs_ or _SSDs_), 
    + Input Devices — e.g. _Keyboard_, _Mouse_, etc.
    + Output Devices — e.g. _Monitor_, _Printer_, etc.; and 
    + Various Peripheral Devices — such as _USB drives_ or _external hard drives_.
  + __Computers do not have a brain__ like human beings.
    + __They have to be given instructions__ on what to do when a particular problem-situation arises
    + __They have to be told everything__, from:
      - _What to expect for data, what type of data_?
      - _How to process it,  How to perform calculations (operations)_? and
      - _Where to store the data_?
    + Humans, understand that language is composed of words which are composed of letters. But, __computers don't understand our language__ nor the words like “hello, good morning, discipline, etc.”.
  * __Computers only understand binary language__ whose vocabulary contains only two letters or states or symbols.
    + i.e. _0 and 1_, _True and False_, _On and Off_.
    + To maintain the states, __transistors are used__ — which are tiny device that are used to __store 2 values__, either a __1 and 0__ or __on and off__.
    + If the transistor is __turned on__, it has a __value of 1__. If it is __turned off__, it has a __value of 0__.
    + e.g. A memory chip contains hundreds of millions or even billions of transistors, each of which can be switched on or off individually. As transistors can store 2 distinct values, we can have millions of different values stored on a memory chip, consisting entirely of 0’s and 1’s.
    + When a very little amount of electric current passes through transistor, it maintains the state of 1. And when there is no electric current, then the transistor has the state of 0.
    + This 0’s and 1’s forms the __building blocks of computers__. With the combinations of 0 and 1 we create a whole new language. For example, 0 can be written as 0.
      - e.g.
        * 1 as 1
        * 2 as 10
        * 3 as 11
        * 4 as 100
        * 5 as 101
        * a as 01100001
        * A as 01000001
  * We, humans, can do everything that we desire and this code can be remembered very easily but we don’t have to remember. We just have to use our language and the software converts our normal letters into the binary language.
    + _Software_ is __a set of instructions__ that tells the computer _what to do, when to do, and how to do_.
    + e.g. Suppose we want to add 2 numbers and want to know what 2 + 2 is. We must give the computer instructions.
    ```
      Step 1: Take the value of 2
      Step 2: Store that value of 2
      Step 3: Add the stored value to 2 by using the addition operator +
      Step 4: Save the answer
    ```
    + Separate instructions are provided for the addition operator + so the computer knows how to do addition when it encounters + sign.
    + A software called the _Interpreter_ interprets our language code into binary code, converting our code into machine language that can be understood by computer.
    > Addition Information: Interpreters do not convert code directly into machine-readable langauge. It converts source code into an Intermediate Language, e.g. bytecode or an Abstract Syntax Tree (AST).
    + When we give input through hardware like keyboard, mouse, scanner, the software interprets it into machine language and then it is processed and our output is shown.
    + Process:
      - If we want to display letter ‘A’ on screen:
      ```
        Step 1: We first open notepad.
        Step 2: Then we will press Capslock or Shift key to make letter uppercase
        Step 3: After that we will press letter ‘a’.
        Step 4: And our screen will show the letter ‘A’.
      ```
    + Under the hood process: When we pressed the capslock or shift key, the software tells that whatever following this keypress should be printed on the screen and after we have pressed the letter a which is small letter, the software first converts it into binary like it had converted the shift or capslock key andthen after the computer understands it prints A on the screen.
- __Features of a Computer__
  * __Processor__:
    + It the __brain of the computer__, carrying out all the __instructions and calculations__ required by the system.
  * __Memory__:
    + The memory, Random Access memory (_RAM_), __stores data temporarily__ for the processor to __access quickly__.
  * __Storage__:
    + Storage devices provide __longterm storage for data and files__.
    + e.g. HDDs, SSDs, external drives
  * __Input devices__:
    + Enable the user to __provide data and instructions to the computer__.
    + e.g. keyboards, mice, scanners, and cameras 
  * __Output devices__:
    + __Displays the results__ of the computer’s processing.
    + e.g. monitors, printers, and speakers 
  * __Operating System__:
    + __Manages the computer__'s resources, controls the hardware, and runs application programs.
  * __Networking__:
    + __Allow computers to communicate and share resources__ with other computers and devices.
  * __Software__:
    + Is the set of instructions that __tell the computer what to do__, and it can range from simple applications to complex programs.
  * __Graphics and Sound__: 
    + Enables the computer to display and manipulate images, and play sounds and videos.
  * __Connectivity__:
    + Features like USB, Wi-Fi, Bluetooth, and Ethernet enable the computer to connect to other devices and the internet.
- __Advantages of Computers__
  * __Increased Efficiency and Productivity__: 
    + Computers can __perform tasks much faster and more accurately__ than humans, allowing for __increased efficiency and productivity__ in various industries.
  * __Storage and Organization of Information__: 
    + __Computers can store large amounts of data and organize__ it in a way that __is easily accessible and searchable__.
  * __Improved Communication__: 
    + Computers __enable people to communicate easily and instantly__ with others, __regardless of their location__.
  * __Access to Information and Resources__: 
    + The internet provides __access to a vast amount of information and resources__ that would otherwise be difficult or impossible to obtain.
  * __Automation of Repetitive Tasks__: 
    + Computers __can automate repetitive and mundane tasks__, __freeing up time and resources__ for more important work.
- __Disadvantages of Computers__
  * __Dependence on technology__: 
    + Over-reliance on computers __can lead to problems if they break down or malfunction__, leading to loss of productivity and data.
  * __Security risks__: 
    + Computers can be __vulnerable to viruses, malware, and hacking__, leading to data breaches and other security risks.
  * __Social isolation__: 
    + The overuse of computers __can lead to social isolation and reduced face-to-face interaction__, leading to social and emotional problems.
  * __Environmental impact__: 
    + The production and disposal of computers __can have a negative impact on the environment__ due to the use of resources and the creation of electronic waste.
  * __Job displacement__: 
    + Automation and the use of computers __can lead to job displacement in certain industries__, requiring workers to adapt to new skill sets or find new employment.

## Introduction to Computer Organization and Computer Architecture
- Computer Organization
  * Scope and Definition
    + Refers to the __physical aspects__ of a _computer system_ — the __organizational units and their interconnections__.
    + It concerns the __computer system's realization and the hardware components' operational behavior__, ensuring __they work together seemlessly__ to perform computational tasks.
  - Key Areas:
    1. __Hardware Components__:
      - __Central Processing Unit__ (_CPU_)
        * Often termed the computer's "brain", the CPU __executes instructions and processes data__.
         It comprises the __Arithmetic Logic Unit__ (_ALU_), __Control Unit__ (_CU_), and registers.
      - __Memory__
        + This includes __Primary Memory__ (_RAM_) for __temporary data storage__ and __Secondary Memory__ (_HDDs_, _SSDs_) for __long-term data storage__.
      - __Input / Output Devices__
        + Peripherals like _keyboards_, _mice_, and _printers_ allow users to __interact__ with the computer and __receive outputs__.
    > Consider a scenario where a user runs a program. The CPU fetches the program's instructions from memory, decodes them, and executes them using its ALU while using the CU to manage data flow to and from memory and I/O devices. 
    2. __Data Paths__:
      - __Buses__
        * These comunication systems __transfer data__ between __inside or outside__ a computer.
        * Types include the:
          + __data bus__ — transfers actual data
          + __address bus__ — carries memory addresses; and
          + __control bus__ — carries control signals
      - __Interconnects__
        * These __link different components__, such as the _CPU_, _Memory_, and _I/O devices_, allowing them to __communicate__.
    > During a memory read operation, the data is transferred from memory to the CPU through the data bus, while the address bus specifies the memory location to be read. 
    3. __Control Signals__
      - These are _electrical signals_ that __coordinate the activities of different computer components__.
      - The _CU_ within the _CPU_ __generates control signals to synchronize the execution of instructions and manage the data flow__.
    > When executing an instruction, the control unit sends a signal to the ALU to perform a specific operation (like addition) and another to the memory to read the required data.
    4. __Memory Management__
      - Involves __strategies for efficient allocation, management, and data retrieval in memory__.
      - Techniques include:
        * __Paging__ — diviing memory into fixed-size pages; and
        * __Segmentation__ — dividing the memory into segments based on program structure.
    > When running multiple programs simultaneously, the operating system manages memory allocation so that each program gets the required memory space, using techniques like paging to ensure efficient use of RAM.
  * Basic Architecture of a Computer
```
                       Basic Architecture of a Computer

                         |-------------------------|
                         |           CPU           |
                         |     |-------------|     |
    Input Devices        |     | |---------| |     |       Output Devices
    |------------|       |     | | Control | |     |       |------------|
    |  Keyboard  |-|     |     | |  Unit   | |     |     |-|  Monitor   |
    |------------| v     |     | |---------| |     |     v |------------|
    |    Mouse   |-|     |     | |   ALU   | |     |     |-|  Printer   |
    |------------| v     |     | |---------| |     |     v |------------|
    |   Scanner  |-|     |     |-------------|     |     |-|  Speaker   |
    |------------| v     |            ^            |     v |------------|
    |  Joystick  |-|-->--|-->-        |        -<--|--<--|-| Headphones |
    |------------|       |   |        v        |   |       |------------|
                         |   v   |---------|   v   |
                         |   |-->|  Memory |<--|   |
                         |       |---------|       |
                         |-------------------------|
``` 
<!--help me, i spent like 20 minutes on this-->

- Computer Architecture
  * Scope and Definition
    + Focuses on the __logical and functional design__ of a computer system.
    + It deals with the __conceptual design and the fundamental operational structure__, which defines _how a computer perform tasks and interacts with software_.
    + The architecture primarily __concerns the programmer's view of the system__ rather than the physical implementation.
  * Key Areas:
    1. __Instruction Sets__
      - The __Instruction Set Architecture__ (_ISA_) defines the set operations that a _CPU_ can perform.
      - It serves as the __interface between software and hardware__, specifying the instructions that can be executed, such as __arithmetic operations, data movement, and control flow__.
    >  The x86 ISA used in most personal computers defines instructions for operations like addition, subtraction, and data movement, which software developers use to write programs. 
    2. __Data Types__
      - Different _CPUs_ support various data types, including __integers__, __floating point numbers__, __characters__, and more complex types like __vectors__.
      - The architecture defines how the system represents and manipulates these data types.
    >  In a CPU designed for scientific computing, floating-point operations are critical, and the architecture will include optimized instructions for handling such data.
    3. __CPU Design__
      - CPU design involves decisions about the:
        * __Number of cores__ 
        * __Pipeline structure__ — how instructions are processed in stages
        * __Branch prediction__ mechanisms; and
        * __Cache hierarchy__
    >  A multi-core CPU can execute multiple instructions simultaneously by assigning them to different cores, increasing overall processing speed. The architecture defines how these cores communicate and share resources. 
    4. __Memory Hierarchy__
      - The memory hierarchy is __organized to balance speed, cost, and size__.
      - It includes:
        * __Registers__ — fastest, most minor
        * __Cache Memory__
        * __Main Memory__ — _RAM_; and
        * __Secondary Storage__ — _HDDs_, __SSDs__
    > The architecture dictates how frequently used data is stored in cache memory to reduce the CPU's time to access it, thereby improving performance. 
  - Memory Hierchy of a CPU        
```

        /\                           /\                        |------|
       /  \                         /  \                       |      |
      /    \                       /    \                      |      |
     /      \                     /      \                     |      |
    /        \                   /        \                    |      |
   /          \                 / Central  \                   |      |
  /            \               / Processing \                  |      |
 /--------------\             /     Unit     \                 |      |
     |      |                /  (registers)   \                |      |
     |      |               /------------------\               |      |
     |      |              /  L1, L2, L3 Cache  \              |      |
     |      |             / Static Random Access \             |      |
     |      |            /         Memory         \            |      |
     |      |           /--------------------------\       \--------------/
     |      |          /        Main Memory         \       \            /
     |      |         /    Dynamic Random Access     \       \          /
     |      |        /             Memory             \       \        /
     |      |       /----------------------------------\       \      /
     |      |      /     Secondary memory (storage)     \       \    /
     |      |     /       magnetic or flash media        \       \  /
     |------|    /----------------------------------------\       \/
   Higher means                                               Lower means
Higher Performance                                          Higher Latency
 Endurance per Bit                                        Higher Persistence
   Higher Speeds
```

- __Common Goals and Interdependence__
  * The overarching goal of both computer organization and architecture is to design an __efficient, cost-effective, and powerful computer system__.
  * An equally well-organized set of hardware must support the design of a computer's architecture to ensure the system functions as intended.
  > In a modern CPU, the pipeline architecture (an architectural feature that allows multiple instructions to be processed simultaneously) must be supported by an organized system of data paths and control signals. This ensures instructions are fetched, decoded, and executed orderly and efficiently, maximizing the CPU’s performance. 
- __Contrast Between Computer Organization and Computer Architecture__
  1. __Computer Organization__:
    * Focuses on the __physical structure and operation__ of the computer's hardware components.
    * Deals with implementation details like __circuit design, timing, and control signals__.
    * Concerned with how components like __CPU, Memory, I/O devices__ are connected and managed.
  > The motherboard layout concerns computer organization, including CPU, memory, and I/O port placement.
  2. __Computer Architecture__
    * Deals with the __design of the system's functional structure__ and behavior.
    * Focuses on what the system does and how it interacts with software, rather than how it is physically implemented.
    * Involves high-level design choices like __Instruction Set designs, CPU architecture, and Memory Hierarchy__.
  > The design of an instruction set that determines how software interacts with the CPU is part of computer architecture. 
- _Intel x86 Architecture_
  * Definition
    + The x86 architecture is a family of instruction set architectures (ISAs) that defines the rules, instructions, data types, registers, and memory addressing modes for Intel processors. 
    + It is essentially a blueprint that specifies what the processor can do.
  * Components:
    + Instruction Set: 
      - The x86 architecture includes a rich set of instructions the processor can execute. 
      - These instructions are fundamental operations like arithmetic (e.g., ADD, SUB), logic (e.g., AND, OR), data movement (e.g., MOV), and control flow (e.g., JMP, CALL).
    + Data Types: 
      - It defines the data types the processor can handle, such as integers, floating-point numbers, and packed data types.
    + Addressing Modes: 
      - The architecture specifies how memory addresses are calculated and accessed, allowing instructions to operate on data differently (e.g., direct, indirect, indexed addressing). 
    + Registers: The architecture defines a set of registers that the processor can use for various operations, such as general-purpose registers, segment registers, and control registers.
- _Intel x86 Organization_
  * Definition: 
    + Processor organization refers to how the architecture's instructions are implemented in hardware. 
    + It involves the physical design of the processor, including the layout and interaction of various subsystems like the pipeline, cache, memory, and execution units.
  * Components:
    + Pipeline Design: 
      - Modern processors use pipelining to execute multiple instructions simultaneously. 
      - The pipeline's depth and the number of stages can affect performance. For instance, an Intel Core i7 processor might have multiple execution pipelines, allowing it to execute several instructions in parallel.
    + Cache Hierarchy: 
      - The processor's cache organization (L1, L2, L3) determines how quickly data can be accessed. 
      - A well-designed cache system reduces latency and improves processing speed.
    + Memory Subsystem: 
      - The organization includes how the processor interacts with RAM and how data is transferred between the CPU and memory. 
      - Features like memory controllers, bandwidth, and latency are critical here.
    + Execution Units: 
      - These parts of the processor carry out the instructions. 
      - A Core i7 processor might have multiple arithmetic logic units (ALUs), floating-point units (FPUs), and other specialized execution units. 
- Key Differences
  * Focus:
    + Architecture: 
      - Concentrates on __what the processor can do__ (instructions, data types, addressing).
    + Organization: 
      - Focuses on __how the processor does it__ (pipeline, cache, memory design).
  * Level of Abstraction:
    + Architecture: 
      - __More abstract__, providing a __general specification that multiple processors can implement__.
    + Organization: 
      - __Concrete__, __dealing with the actual hardware design and implementation__ of a specific processor.
  * Flexibility:
    + Architecture: 
      - Can be __applied to different processors__ across different generations (e.g., Pentium, Core, Xeon).
    + Organization: 
      - __Specific to a particular processor__ or family of processors (e.g., Intel Core i7, i9). 
- Conclusion
  * Understanding the distinction between Computer Organization and Architecture is critical for anyone designing, constructing, or programming computer systems. Both fields are interdependent, with the effectiveness of one relying on the soundness of the other. Mastery of these concepts equips students with the knowledge to design, analyze, and optimize modern computer systems, ensuring they meet desired performance, cost, and power consumption goals.

## Computer Organization vs Computer Architecture
- Computer Organization
  * Definition
    + Delves into the __physical components and their interconnections__ that make up a computer system.
    + It is about understanding how the __hardware is put together and how it functions__.
  * Scope
    + Its primary scope encompasses __the structural elements of a computer__, inclusing the _CPU_, _Memory_, _I/O devices_, and the data pathways — _buses_ that connects them.
  * Concerns
    + The primary concerns revolve around the __effective utilization of hardware resources__. 
    + This includes __optimizing memory access, data storage, and the efficient connection of peripheral devices__ to the computer.
  * Design Focus
    + At its core, computer organization is all about __ensuring that these hardware components work harmoniously__.
    + It places significant emphasis on __resource management and the efficient transfer of data__ between various components.
  * Level
    + Operating at a practical, hands-on level, computer organization __deals with the physical hardware-components, circuits, and the way they are physically interconnected__ within a computer system.
    + It is about understanding the nuts and bolts of computer technology.
- Computer Architecture
  * Definition
    + Focuses on the __high-level design and the conceptual framework structure__ of a computer system.
    + It defines the __logical organization and framework__ of how the computer functions.
  * Scope
    + The __scope extends to the broader scope of the computer__, including the design of the __ISA, memory hierarchy, and how data is processed__.
  * Concerns
    + Its primary concern is __providing a logical framework__ for the computer's operation.
    + This includes aspects like __how instructions are executed, how data is moved within the system, and how control flows through the computer__.
  * Design Focus
    + Rather than being fixated on the physical hardware, computer architecture concentrates on __creating a user-friendly, efficient, and abstracted model__ of the computer system.
    + It aims to make the computer operation __understandable and manageable__ for both users and programmers.
  * Level
    + Operating at a more abstract level, computer architecture __deals with the logical structure__ of the computer system.
    + It emcompasses how __software interacts with the hardware__, and it aims to provide a high-level perspective on the computer's operation.
- Comparison:
  * Both computer organization and computer architecture are __essential components__ of the field of computer science and engineering. They are __intrinsically related__, as __decisions made at the architectural level can significantly influence the organization, and vice versa__.
  * Their common goal is to __ensure that a computer system functions effectively, efficiently, and reliably__.
  * The interdependence of these two fields lies in the fact that __decisions made at the architectural level can impact how the organization is configured__. They work in tandem to improve the overall performance and functionality of a computer system.
- Contrast:
  * While _computer organization_ __deals with the practical, physical aspects of a computer system__, _computer architecture_ __focuses on the logical and conceptual aspects__.
  * Computer organization's concerns __revolve around resource management and physical connectivity__, while computer architecture __deals with the high-level design and operation__ of the computer system.
  * Computer organization __answers the "how" questions regarding how hardware components are connected and work together__. In contrast computer architecture addresses the __"what" questions about what the components do and how they are controlled__.
  * Computer organization operates at a more concrete and hands-on level, __focusing on the physical aspects__. On the other hand, computer architecture operates at a more abstract level, __concentrating on the logical and high-level design__ of the computer system.
- Conclusion
  * Computer organization and computer architecture are __closely related but distinct areas__ within the realm of computer science. Computer organization deals with the __physical and practical aspects of hardware design__, while computer architecture __deals with the logical and conceptual framework__ of a computer system. Together, they ensure that computers are not only __efficient and reliable but also capable of executing a wide range of tasks__, making them indispensable in the world of technology.