### < [Back](./CSP103.md)
# > [CSP103](./CSP103.md) - Architecture and Organization
### notes
---
## Lesson 1
### What is Computer?
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

### Features of Computers
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
### Advantages of Computers
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
### Disadvantages of Computers
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
### Scope of Computer Organization
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
![[../.images/CSP103/CSP103-0.png]]
### Scope of Computer Architecture
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
![[../.images/CSP103/CSP103-1.png]]
### Common Goals and Interdependence
  * The overarching goal of both computer organization and architecture is to design an __efficient, cost-effective, and powerful computer system__.
  * An equally well-organized set of hardware must support the design of a computer's architecture to ensure the system functions as intended.
  > In a modern CPU, the pipeline architecture (an architectural feature that allows multiple instructions to be processed simultaneously) must be supported by an organized system of data paths and control signals. This ensures instructions are fetched, decoded, and executed orderly and efficiently, maximizing the CPU’s performance. 
### Contrast Between Computer Organization and Computer Architecture
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

## Lesson 2
### Introduction to Computer Components
- Central Processing Unit (CPU)
	- the brain of the computer
	- responsible for executing instructions, performing calculations and manageing data flow
	- a complex microprocessor composed of millions of transistors
	- plays a central role in the functioning of the computer
	- has three main parts
		- Arithmetic Logic Unit (ALU)
			- performs all arithmetic operations
			- Addition, Subtraction, Multiplication, and Division
			- performs logic operations
			- greater than, less than, or equal to
			- crucial for processing numerical data and making decisions based on logic
		- Control Unit (CU)
			- controlliing the data flow between the CPU, memory, and i/o devices
			- fetches instructions from memory
			- decodes them to determine the required actions
			- executes them by the ALU or the other components
		- Registers
			- are small, fast storage locations
			- temporarily hole data and instructions that are being processed
			- plays a vital role in the CPU's abilitu to quickly access and manipulate data
			- allows for efficient execution of instructions
- Memory (RAM)
	- RAM is the computer's short term memory
	- used to store data actively being processed by the CPU
	- RAM is volatile, losing data when power is turned off
	- the speed and capacity of RAM directly influences the computer's performance
	- determinces how quickly the CPY can access data and how much data is accessed simultaneously
	- if the RAM is full, the system may slow down and will rely on slower storage devices
	- has two types
		- Dynamic RAM
			- the most comon type of RAM
			- needs to be refreshed thousands of times per second
			- it stores all bit of data in a tiny capacitor
		- Static RAM
			- faster and more expensive than DRAM
			- used for cache memory
			- provides high-speed CPU data acces
- Input & Output Devices
	- are peripherals that allow users to interact with the computer
	- enables data input and output, to and from the system
	- input devices
		- converts user actions into data that the computer can process
		- keyboards. mice, scanners, microphones
	- output devices
		- converts processed data from the computer into a form that users can understand or interact with
		- monitors, printers, speakers
- Storage Devices
	- holds data permanently or semi-permanently
	- information is retained even when the computer is powered off
	- varies in speed, capacity, and technology
	- types of storage devices
		- Hard Disk Drives (HDDs)
			- uses magnetic storage to read and write data on spinning disks or platters
			- more storage at lower costs but are slower that newer technologies
			- usually stores documents, photos, and videos
		- Solid-State Drives (SSDs)
			- uses flash memory
			- faster access and excelent reliability than HDDs
			- hae no moving parts, making it more durable and energy efficient
			- more expensive per gigabyte
			- usually stores the Operating System for fast response and boot times
		- Optical Drives (CDs, DVDs, Blu-rays)
			- uses lasers to write or read data on disks
			- less common due to digital distribution
			- used for installing software, playing media, and archiving data
			- installing a program from a DVD, the data reads from the disk and transfer it to the computer's storage
		- Flash Drives
			- portable storage devices, using flash memory
			- ideal for transferring files between computers
			- small, durable, and do not need external power sources
			- used to carry important documents or presentations that can be accessed on multilple computers
- Buses
	- communication pathways
	- connects compter components, allowing communication and transferring of data efficiently
	- types of buses
		- Data bus
			- carries actual data
			- between the CPU, memory, and other peripherals
			- the width of the data bus, affects the amount of data that can be transfered
		- Address bus
			- carries memory addresses
			- are a location in memory where data should be read from or written to
			- this bus only transfers memory addresses
		- Control bus
			- carries control signals
			- manges the operations across the computer's components
			- coordinates activities like reading and writing from memory, or responding to input devices

## Lesson 3
### __Introduction to Standard Organizations__
- Background:
	- Standard organizations in computing play a pivotal role in ensuring that technologies across different platforms can communicate, integrate, and evolve cohesively.
	- These organizations set the groundwork by defining protocols, guidelines, and specifications that fosther interoperability, enhance safety, and streamline global technological advancements.
### Importance of Standards in Computing
- standards are essential
- they lay out the foundation for coorperation between software and hardware.
- it ensures that they work together efficiently
- key areas:
	- Interoperability
		- ensures that different devices, software, and system can communicate and work together seemlessly
		- e.g. tcp/ip enables consistent internet functionability
	- Quality and Safety
		- benchmarks product performance and safety
		- e.g. cybersecurity protect users from cyber threats and ensures their safety
	- Facilitating Innovation
		- establish clear frameworks for development
		- enables technologies that work harmoniously with existing systems
	- Compatibility
		- ensures backwards and forwards compatibility
		- e.g. usb 3.0 works with usb 2.0
### Computer Organization Standards
- governs a computer system's key components and operations within a computer organization
- these standards are critical for ensuring that all components communicate efficiently and operate reliably
- categories of standards
	- Bus Standards
		- are communication pathways that transfer data between computer components
		- define how comonents communicate
		- common bus standards:
			- __Peripheral Component Interconnect__ (_PCI_)
				- A standard for __connecting peripheral devices__.
			- __Peripheral Component Interconnect Express__ (_PCIe_)
				- An advanced version of _PCI_, offering __faster data transfer rates__.
			- __Universal Serial Bus__ (_USB_)
				- A __standard for connecting external devices__, such as keyboards, printers, and storage devices.
	- Memory Standards
		- ensures that memory devices work effectively
		- defines from physical dimensions to electrical characteristics, speeds, and capacities
		- common memory standards:
			- _DDR4/DDR5_
				- Stands for __Double Data Rates__
				- High-speed RAM standards __used in most modern computers__.
			- _SDRAM_
				- Stands for __Synchronous Dynamic Random Access Memory__.
				- Used in __older data storage and management systems__.
			- _ECC Memory_
				- Stands for __Error-Correcting Code Memory__.
				- A specialized memory standard used in servers for __detecting and correcting memory errors__.
	- Display Standards
		- governs how computers transmit visual data to monitors
		- or to other output devices
		- ensures that display output is consistent
		- regardless of manufacturer and device type
		- common display standards:
			- _VGA_
				- Stands for __Video Graphics Array__.
				- An __older analog display standard__. 
			- _DVI_
				- Stands for __Digital Visual Interface__.
				- A __digital interface for video__.
			- _HDMI_
				- Stands for __High-Definition Multimedia Interface__.
				- The __modern standard__ for high-quality digital video and audio transmission.
			- __DisplayPort__
				- Another digital display standard __commonly used in highend monitors__.
	- Networking Standards
		- dictates how data is transmitted across networks
		- whether locally (home network) or globally (internet)
		- enable various devices to communicate over wired or wireless networks
		- common network standards:
			- __Ethernet__ (_IEEE 802.3_)
				- A standard for __wired LAN communication__.
			- __Wi-Fi__ (_IEEE 801.11_)
				- Short for __Wireless Fidelity__.
				- Standards for __wireless network communications__.
			- __Bluetooth__
				- A wireless communication standard for __short-range data exchange__.
- Main Organizational Standards:
	- various organizations oversee the development of computer standards
	- significant standard organizations:
		- __International Organization for Standardization__ (_ISO_)
			- Develops and publishes standards that affect various industries, including computing, ensuring compatibility and safety on a global scale.
		- __International Electrical and Electronics Engineers__ (_IEEE_)
			- One of the larges organizations that set standards for electronic and electrical technologies.
			- It includes widely-used networking protocols like Ethernet (_IEEE 802.3_) and Wi-Fi (_IEEE 801.11_).
		- __American National Standards Institute__ (_ANSI_)
			- Aligns US industry standards with global norms, ensuring that American products and companies remain competitive.
		- __World Wide Web Consortium__ (_W3C_)
			- Establishes and maintains web standards like _HTML_, _CSS_, and _XML_.
			- Ensuring that the web functions uniformly across all browsers and platforms.
		- __International Telecommunication Union__ (_ITU_)
			- This organization focuses on developing global standards for telecommunications.
			- Ensuring that communication systems worldwide remain compatible and efficient.

| Organization | Full Name                                         | Founded | Primary Focus                                                  | Key Standards                                            | Scope                    | Notable Contibutions                                                                                    |
| ------------ | ------------------------------------------------- | ------- | -------------------------------------------------------------- | -------------------------------------------------------- | ------------------------ | ------------------------------------------------------------------------------------------------------- |
| ISO          | International Organization for Standardizations   | 1947    | Global standards across various industries                     | ISO/IEC 27001 (Information Security Management)          | International            | Developed numerous computing standards, including quality and security standards (ISO 9000, ISO 27000). |
| IEEE         | International Electrical and Electonics Engineers | 1963    | Electrical, electronic, computing, and networking              | IEEE 802.3 (Ethernet), IEEE 802.11 (Wi-Fi)               | International            | Major contributions in network protocols like Ethernet and Wi-Fi.                                       |
| ANSI         | American National Standards Institutes            | 1918    | U.S. national standards and alignment with international nurms | ANSI C (Programming Language), ANSI SQL (Databases)      | National (United States) | Prominent in standardizing programming languages like C and SQL                                         |
| ITU          | International Telecommunications Union            | 1865    | Telecommunications and radio communications                    | ITU-T (Telecom Standards), ITU-R (Radio Frequencies)     | International            | Critical in defining telecom and broadcast standards globally.                                          |
| W3C          | World Wide Web Consortium                         | 1994    | Web technologies and internel standards                        | HTML, CSS, XML, HTTP                                     | International            | Shaped the modern web by creating core web standards like HTML and CSS                                  |
| IETF         | Internet Engineering Task Force                   | 1986    | Internet and networking protocols                              | TCP/IP, HTTP/2, DNS                                      | International            | Key contributor to the development of the internet and network protocol standards.                      |
| ECMA         | European Computers Manufacturers Association      | 1961    | Information technology and consumer electronics                | ECMAScript (JavaScript), ECMA-262 (Scripting Language)   | International            | Responsible for standardizing JavaScript, a critical web technology.                                    |
| VESA         | Video Electronics Standards Association           | 1989    | Video and display technologies                                 | DisplayPort, EDID (Extended Display Identification Data) | International            | Developed the DisplayPort standard for video displays.                                                  |
| T10          | Technical Committee T10                           | 1962    | Storage interfaces and protocols                               | SCSI (Small Computer System Interface)                   | International            | Created and maintained the SCSI storage standard, a critical protocol for hard drives.                  |
| JEDEC        | Joint Electron Device Engineering Council         | 1958    | Semiconductor memory and microelectronics                      | DDR RAM standards (DDR, DDR2, DDR3, DDR4                 | International            | Established the widelyused DDR memory standards for computers.                                          |

### __Strengths of Standard Organizations__
- __Global Cooperation__
	- Standard organizations encourage cooperation across countries and industries.
	- Ensuring that new technologies work globally.
- __Product Compatibility__
	- Standards ensure that devices, software, and systems from different manufacturers and regions can interoperate smoothly.
- __Innovation and Competition__
	- By providing a level playing field, standards encourage competition and innovation, enabling new technologies to emeger while maintaining interoperability.
- __Compliance and Safety__
	- Standards often enforce compliance with safety, security, and enviromental regulations, reducing risks for consumers and industries.
### __Weakneses and Challenges__
- __Slow Process__
	- Consensus-based decision-making can slow down the creation of new standards, meaning that it can take years for new technologies to become standardized. 
- __High Compliance Costs__
	- Adhering to standards can be costly for companies, especially small businesses, which may struggle with the expense of certifications, product redesign, or testing. 
- __Conflicting Regional Standards__
	- Sometimes, regional standards (e.g., European versus global standards) create conflicts, causing additional costs and complexities for manufacturers trying to meet all requirements. 
- __Resistance from Stakeholders__
	- Some companies may resist adopting new standards, especially if it involves replacing or upgrading existing proprietary systems they've invested heavily in.

## Lesson 4
1. Pascaline and Stepped Reckoner
	- Pascaline (1642)
		- Blaise Pascal
		- one of the earliest mechanical calculators
		- designed to assist Pascal's father with arithmetic calculations
		- it was a series of wheels and gears to perform addition and subtraction
		- featured dials a gears that could be manipulated to add or subtract numbers
		- represents the foundational concepts of mechanizing arithmetic operations
		- demonstrated the potential of mechanical devices
		- it reduced human error and provided a new level of computational efficiency
	Stepped Reckoner (1672)
		- Gottfried Wilhelm Leibniz
		- improved upon Pascal's design
		- enabling multiplication and division
		- introduced the concept of stepped drum mechanism
		- influential in the development of future mechanical computations
		- uses a series of rotating drums with varying steps to perform arithmetic operations
		- its ability to perform a broader range of calculations laid the groundwork for future developments and innovations
2. Charles Babbage's Analytical Machine
	- Analytical Machine (1837)
		- Charles Babbage
		- general-purpose mechanical computer
		- introduced the ALU, memory
		- control flow via loops and conditionslas
		- never completer but revolutionary
		- uses puched cards for input
		- ALU for calculations
		- separate memory for data storage
		- its architecture is similar to moderm computers, with programmability
		- Babbage's ideas were decades ahead of its time
		- precursor to the moderm computer
3. Paradigm shift: mechanical to electronic computation
	- Electrical Numerical Integrator and Computer (1945)
		- first large-scale electronic digical computer
		- designed to compute artillery firing tables for the US army
		- uses vacuum tubes instead of mechanical parts, shifted to electronic
		- allows for significantly faster calculations, higher sppeds and more complex calculations
		- momentual leap in computing technology
		- demonstrated the potential of electronic digial computers
		- performs complex calculations and solve real-world problems more efficiently
4. von Neumann Architecture and the Stored Program Concept
	- von Neumann Architecture (1945)
		- John von Neumann
			- introduced the concept of storing program instructions in memory alongside data
			- allowed computers to switch between tasks with physical reconfiguration
			- introduced the CPU that performs computations and executes instructions 
			- memory unit for storing data and instructions
			- i/o for interaction with the external world
			- the architecture become the foundation for modern designs
			- enables versatility in computing tasks
			- formed the basis for subsequent computer and software development
5. Microcomputer Revolution
	- Microcomputers (1970s-1980s)
		- development of microprocessors in the 1970s, like the Intel 4004
		- led to the creation of small affordable computers for personal use
		- examples:
			- Altair 8800 (1975)
				- first commercially successful personal computer
				- marked the beginning of the pc use
			- Apple I (1976)
				- developed by Steve Jobs and Steve Wozniak
				- Apples first product introduced personal computing to the wider audience
			- IBM PC (1981)
				- standardized personal computing
				- set the stage for modern PCs with its open architecture and wide adoption
		- MCs democratized computing
		- made it accessible to individuals and small businesses
		- layed the foundation for the personal computing industry
6. Impact of Modern Devices on Personal Computing
	- Mobile Computing
		- devices like smartphones and tablets
		- the shift from traditional desktops to mobile devices transformed personal computing
		- integrated communication and computing functions into portable devices
		- early laptops paved way for smartphones
		- offered computing tasks in a compact form
		- mobile devices have revolutionized how users work, communicate, and access to information
		- driven the rise of work, cloud computing and the gig economy
		- made computing more versatile and accessible
		- influenced how people interact with technology and each other
- Convergence on Computing Technologies: Supercomputers and Mobile Devices
	- Supercomputers and Mobile Devices
		- supercomputers used to solve complex scientific problems
		- mobile devices designed for personal use
		- both utilize similar advanced technologies such as parallel processing, and high efficiency power management
		- technological convergence
			- Cloud Computing:
				- Allows mobile devices to offload tasks to remote servers, enhancing performance and capabilities.
			- Edge Computing:
				- Brings processing closer to the user, enabling realtime data analysis and applications.
		- the convergence highlights the interconnected bature of modern computing systems and their collective advancements in efficiency and capability