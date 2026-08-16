# Notes
## What is Computer?
- an __electronic device that can process and store information__
- __performs calculations, manipulate data, execute instructions__ to accomplish specific tasks
- computers __do not have a brain__, they have to be __given instructions__, and __they have to be told everything__ from:
  * _what to expect for data, and what type of data?_
  * _how to process and how to perform operations?_
  * _where to store the data?_
- computers do not understand our language, only __binary languages__ — ones and zeroes
  * transistors are __used to maintain states__ — __1 is on, 0 is off__
  * these are the __building blocks of computers__
- software is __a set of instructions__, telling the computer __what to do, when to do, and how to do__
  * interpreter — interprets code from human-readable form into code that a computer can understand

## Features of Computers
  * processors — brain of the computer, carries out instructions and calculations
  * memory — RAM, stores data temporarily and being accessed quickly
  * storage — HDDs and SSDs, longterm storage for data and files
  * input devices — provide data and instruction to the computer
  * output devices — displays the result of the computer's processing
  * various peripheral devices
  * OS — manages the computer's resources, controls the hardware and runs application programas
  * networking — allows commucation and sharing or resources to other computers
  * software — tells the computer what to do
  * graphics and sound — displays images, play sounds and videos
  * connectivity — USB, WiFi, Bluetooth, and Ethernet enable connecting with other devices

## Advantages of Computers
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
## Disadvantages of Computers
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

## Scope of Computer Organization
  * physical aspects or components of a computer system 
  * the organizational units and their interconnections
  * concerns the computer system's realization and the hardware components' operational behavior
  * ensures they work seemlessly
  * how the hardware is put together and how it functions
  * structural elements of a computer, cpu, memory, i/o devices
  * effective utilization of hardware resources
  * ensures that hardware components work harmoniously
  * optimizing memory access, data storage and efficient commucation of peripheral devices
  * resource management and the efficient transfer of data
  * key areas
    1. hardware components
      - cpu
        * executes and processes data
        * comprises of ALU, CU and registers
      - memory
        * primary memory for temporary data storage
        * secondary memory for long term data storage
      - input / output devices
        * input — interact
        * output — receive outputs
    2. data paths
      - buses
        * transfer data between inside or outside a computer
          + data bus — transfers data
          + address bus — transfers memory addresses
          * control bus — carries control signals
      - interconnects
        * links different components, allowing them to communicate
        * like cpu, memory, and i/o
    3.  control signals
      - are electrical signals
      - coordinates the activities of different computer components
      - the CU generates control signals
      - synchronizes execution of instructions and data flow
    4. memory management
      - strategies for efficient allocation, management, and data retrieval
      - techniques
        * paging — dividing memory in fixed-size pages
        * segmentation — dividing memory into segments based on the program structure
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
## Scope of Computer Architecture
  * logical and functional design;
  * provides logical framework for computer operation
  * conceptual design and the fundamental operational structure
  * defines how a computer perform tasks and interact with software
  * concerns the programmer's view of the system rather than the physical implementation
  * high-level design and conceptual framework structure
  * defines the logical organization and framework of how the computer functions
  * scope extends to the broader scope of the computer, design like ISA, memory hierarchy, and how data is processed
  * creates a user-friendly, efficient, and abstracted model: understandable and manageable
  * how software interacts with hardware
  * key areas
    1. instruction sets
    - ISA defines a set of operations
    - serves as the interface between the software and hardware
    - instructions such as arithmetic operations, data movement and control flow
    2. data types
    - different cpus have various data types
    - ints, floats, chars, and vectors
    - defines how the system represents and manipulates data types
    3. cpu design
    - number of cores
    - pipeline structure — how instructions are processed in stages
    - branch prediction mechanisms
    - cache hierarchy
    4. memory hierarchy
    - registers — fastest and most minor
    - cache memory — L1, L2, L3
    - main memory — RAM
    - secondary storage — HDDs, SSDs
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
Higher Performance                                           Higher Latency
 Endurance per Bit                                         Higher Persistence
   Higher Speeds
```
## Common Goals and Interdependence
  * The overarching goal of both computer organization and architecture is to design an __efficient, cost-effective, and powerful computer system__.
  * An equally well-organized set of hardware must support the design of a computer's architecture to ensure the system functions as intended.
  > In a modern CPU, the pipeline architecture (an architectural feature that allows multiple instructions to be processed simultaneously) must be supported by an organized system of data paths and control signals. This ensures instructions are fetched, decoded, and executed orderly and efficiently, maximizing the CPU’s performance. 
## Contrast Between Computer Organization and Computer Architecture
1. computer organization
  + physical structure and operation of the hardware components
  + deals with implementation details like circuit design, timing and control signals
  + concerned with how components like cpu, memory, and i/o devices are connected and managed
  + how the processor does it
  + how the hardware components are connected and work together
  + more concrete, dealing with the hardware design and implementaion of a specific processor
  + specific to a particular processor
2. computer architecture
  + design of the system's functional structure and behavior
  + what the system foes and how it interacts with software
  + involves high-level design choices like Instruction Set designs, cpu arch, and memory hierarchy
  + what the processor can do;
  + what the components do and how they are controlled
  + more abstract, general specification that multiple processors can implement
  + applied to different processors