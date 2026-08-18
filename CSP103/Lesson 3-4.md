### [Table of Contents](main.md)
# CSP103
---
## Target
- Learning Outcomes
  * Identify the main components of a computer system, including the Central Processing Unit (CPU), memory (RAM), input/output devices, storage devices, and buses.
  * Explain, describe, or identify the function of the computer components in the overall operation of a computer system. 
  * Explain the importance of standards in computing and their role in ensuring interoperability, consistency, and innovation.
  *  Identify key computer organization standards and describe their impact on the development and compatibility of computer systems.
- Topics
  3. Introduction to Computer Components
    + 3.1.Central Processing Unit (CPU)
    + 3.2.Memory (RAM)
    + 3.3.Input and Output Devices
    + 3.4. Storage Devices
    + 3.5.Buses (Data Pathways)
  4. Introduction to Standard Organizations
    + 4.1.Importance of Standards in Computing
    + 4.2.Computer Organization Standards
    + 4.3. Strengths of Standard Organizations
    + 4.4.Weaknesses and Challenges
## __Introduction to Computer Components__
- Background
  + The foundational components of a computer are essential for understanding its operations and functionalities. This lecture will intoduces key elements that make up a computer system; the Central Processing Unit (CPU), Memory (RAM), Input and Output Devices, Storage Devices, and Buses (Data Pathways).
  + Each componnet is crucial to the computer's ability to process data, store information, and interact with users. 
  + By understanding these components, certain insight will be gained into how computers perform tasks, manage resources, and support various applications.
- Diagram
  ![[CC104-0.png]]
### __- Central Processing Unit (CPU)__
- Definition:
  * The _CPU_ is often called the "__brain__" of the computer, as it is __responsible for executing instructions, performing calculations, and managing data__ flow within the system.
  * It is a _complex microprocessor_ composed of __millions of transistors__, and it plays a __central role in the functioning__ of the computer.
- It has three main parts:
  1. __Arithmetic Logic Unit__ (_ALU_)
    + Definition: 
      - The _ALU_ is the _CPU_ component that __performs all arithmetic operations__—_Addition, Subtraction, Multiplication, and Division_—and logical operations, such as comparisons like _significant than, less than or equal to_.
      - It is crucial for __processing numerical data__ and __making decisions baed on logic__.
    + Example:
      - When a program requires calculation, such as adding two numbers, the ALU performs the operation and stores the result in a register or memory location for future use.
  2. __Control Uunit__ (CU)
    + Definition:
      - The _CU_ directs the _CPU_'s operarions by __controlling the data flow__ between the __CPU, memory, and input/output devices__.
      - It __fetches instructions__ from memory, __decodes them__ to determine the required actions, and the __executes them__ by the _ALU_ and other components.
    + Example:
      - If a program instructs the computer to read data from memory, the _CU_ fetches the instruction, decodes it to understand that data needs to be read, and the sends signals to the appropriate components for the operation.
  3. __Registers__
    + Definition:
      - _Registers_ are __small, fast storage locations__ within the _CPU_ that __temporarily hold data and instructions__ that are being processed.
      - It plays a vital role in the _CPU_'s ability to __quickly access__ and __manipulate data__, aloowing for efficient execution of instructions.
    + Example:
      - When calculating, the CPU may store intermediate results in registers to speed up the process and reduce the need to access slower memory location
- Diagram:
	 ![[CSP103-4.png]]
### __- Memory__
- Definition:
  * __Random Access Memory__ (_RAM_) is the computer's __short-term memory__, used to __store data actively being processed__ by the CPU.
  * _RAM_ is __volatile__, meaning it loses all stored data when the power is turned off.
  * The __speed__ and __capacity__ of _RAM_ directly __influence the computer's performance__, as it determinces how quickly the _CPU_ can access data and how much data can be processed simultaneosuly.
  * When an application is opened, the operating system loads the application's data and code into _RAM_, allowing the _CPU_ to access and execute the necessary instructions quickly.
  * If the RAM is complete (full), the system may slow down, as it has to rely on slower storage devices (swaps or pagefiles) to store overflow data.
- It has two types:
  * __Dynamic Random Access Memory__ (_DRAM_)
    + The __most common type__ of _RAM_, used in most computers and devices.
    + _DRAM_ needs to be __refreshed thousands of times per second__, as it __stores each bit of data in a tiny capacitor__.
  * __Static Random Access Memory__ (_SRAM_)
    + __Faster and more expensive__ than _DRAM_, used for __cache memory, providing high-speed CPU data access__.

### __- Input & Output Devices__
- Definition
  * __Input and Output (_I/O_) Devices__ are the __peripherals that allow users to interact__ with the computer, enabling __data input and output__, __to and from the system__.
- __Input Devices__
  * Definition
    + __Converts user actions into data__ that the computer can process.
    + These devices include __keyboards, mice, scanners, microphones, cameras__, etc.
    + They are __essential for entering data, controlling applications, and providing instructions__ to the computer.
  * Example:
    + When typing a document, each keystroke on the keyboard is converted into digital signals that the _CPU_ can process, displaying the corresponding character on the screen.
- __Output Devices__
  * Definition
    + __Converts processed data from the computer into a from that users can understand or interact with__.
    * Typical output devices include __monitors__ for visual display, __printers__ for physical copies of documents, and __speakers__ for audio output.
  * Example:
    + After typing a document, a printer might be used. The _CPU_ sends the processed data to the printer, procuding a physical document copy.
- Diagram:

	![[CSP103-5.jpg]]
### __- Storage Devices__
- Definition:
  * Are responsible for __holding data permanently or semi-permanently__, ensuring tha information can be __retained even when the computer is powered off__.
  * _Storage devices_ __vary in speed, capacity, and technology__.
- Types of Storage Devices:
  * __Hard Disk Drives__ (_HDDs_)
    + Uses __magnetic storage__ to read and write data on __spinning disks__ (_platters_).
    + They offer ample storage capabilities at a __lower costs__ but are __slower__ than newer technologies.
    > An operating system and most files, such as documents, photos, and videos, are typically stored on an HDD.
  * __Solid-State Disks__ (_SSDs_)
    + Uses __flash memory__ to store data providing __faster access and excellent reliability than HDDs__.
    + _SSDs_ have __no moving parts__, which make the more __durable and energy-efficient__, but they are usualle __more expensive__ per gigabyte.
    > An SSD often stores the operating system and frequently accessed applications, significantly speeding up boot and program loading times.
  * __Optical Drives__ (_CDs_, _DVDs_, _Blu-rays_)
    + Uses __lasers__ to read and write data on __disks__, such as _Compact Disks, Digital Video Disks_, and _Blu-rays_.
    + Altough __less common__ today due to digital distribution, there are still __used for installing software, playing media, and archiving data__.
    > When you install a program from a DVD, the optical drive reads the data from the disc and transfers it to your computer’s storage. 
  * __Flash Devices__
    + Are __portable storage devices__ that use __flash memory__, making them ideal for __transferring files between computers__.
    + They are __small, durable__, and __do not require external power sources__.
    > You might use a flash drive to carry important documents or presentations that you need to access on different computers.
- Diagram:
	 ![[CSP103-6.png]]

### __- Buses (Data Pathways)__
- Definition
  * Are __communication pathways__ that __connect computer components__, allowing them to __communicate and transfer data efficiently__.
- Types of Buses:
  * __Data Bus__
    + Carries __actual data between the CPU, memory, and other peripherals__.
    + The width of the data bus — the number of bits that it can carry — affects the amount of data that can be transfered simultaneously.
    >  When the CPU reads data from memory, the data bus transfers the data from the memory to the CPU for processing.
  * __Address Bus__
    + Carries __memory addresses__, which specify the __location in memory where data should be read from or written to__.
    + Unlike the data bus, the address bus typically only transfers memory addresses.
    > When the CPU needs to access data stored in a specific memory location, it sends the address of that location over the address bus.
  + __Control Bus__
    + Carries __control signals__ that __manage the operations__ across the computer's components.
    + This signals __coordinate activities__ like reading from memory, writing to memory, and responding to input devices.
    > During a memory read operation, the control bus sends signals that trigger the memory to place the requested data onto the data bus for the CPU to read.
- Diagram:
	![[CSP103-7.png]]

## Introduction to Standard Organizations
- Background:
	- Standard organizations in computing play a pivotal role in ensuring that technologies across different platforms can communicate, integrate, and evolve cohesively.
	- These organizations set the groundwork by defining protocols, guidelines, and specifications that fosther interoperability, enhance safety, and streamline global technological advancements.
### Importance of Standards in Computing
- Definition:
	- __Standards are essential__ for creating a harmonized digital ecosystem. They lay the __foundation for cooperation between hardware and software systems__, ensuring they __work together efficiently__.
- Key areas:
	- __Interoperability__
		- Standards ensure that __different devices, software, and systems can communicate and work together seemlessly__.
		- For instance, the _TCP/IP_ protocol __enables consistent internet functionality__ worldwide.
	- __Quality and Safety__
		- Standards __benchmark product performance and safety__.
		- For example, cybersecurity standards ensure that products meet specific criteria to__ protect users from cyber threats and safety__.
	- __Facilitation Innovation__
		- Standards __establish clear frameworks for development__, enabling innovators to create technologies that __work harmoniously with existing systems__.
	- __Compatibility__
		- Standards ensure both __backward and forward compatibility__, maintaining the utility of older technologies.
		- For instance, devices using USB 3.0 are still often compatible with USB 2.0 ports.
### Computer Organization Standards
- Definition:
	- Several types of standards governs a computer system's key components and operations within a computer organization.
	- These standards are critical for ensuring that all components communicate efficiently and operate reliably.
- Categories of Standards in Computer Organization:
	- Bus Standards
		- Definition:
			- Buses are the communication pathways that transfer data between computer components.
			- The bus standards define how components like the CPU, memory, I/O devices and other peripherals communicate.
		- Common Bus Standards:
			- Peripheral Component Interconnect (PCI)
				- A standard for connecting peripheral devices.
			- Peripheral Component Interconnect Express (PCIe)
				- An advanced version of PCI, offering fater data transfer rates
			- Universal Serial Bus (USB)
				- A standard for connecting external devices, such as keyboards, printers, and storage devices.
		- Example:
			- PCIe is a high-speed bus standard widely used in modern computers to connect the CPU, with high-performance components like graphics cards, SSDs, and network cards.
	- Memory Standards
		- Definition:
			- Memory standards ensure that memory devices—such as RAM, work effectively withother system components.
			- It defines everything from physical dimensions to electrical characteristics, speeds, and capacities.
		- Common Memory Standards:
			- DDR4/DDR5
				- High-speed RAM standards used in most modern computers.
			- SDRAM
				- Stands for Synchronous Dynamic Random Access Memory.
				- Used in older data storage and management systems.
			- ECC Memory
				- Stands for Error-Correcting Code Memory.
				- A specialized memory standard used in servers for detecting and correcting memory errors.
		- Example:
			- Double Data Rate (DDR) standards govern how RAM modules communicate with the CPU.
			- Current standards include DDR4 and DDR5, which differ in data transfer rates and power consumption.
		- Diagram:
			- ![[CSP103-8.png]]
	- Display Standards
		- Definition:
			- Governs how computers transmit visual data to monitors and other output devices.
			- These standards ensure that the display output is consistent, regardsless of the manufacturer and device type.
		- Common Networking Standards
		- Example:
			- Ethernet (IEEE 802.3)
				- A standard for wired LAN communication.
			- WI-Fi (IEEE 801.11)
				- Short for Wireless Fidelity.
				- Standards for wireless network communications.
			- Bluetooth
				- A wireless communication standard for short-range data exchange.
		- Diagram:
			![[CSP103-9.png]]
- Main Organization Standards:
	- Background:
		- Various organizations oversee the development of these computing standards.
	- Some of the significant standard organizations include:
		- International Organization for Standardization (ISO)
			- Develops and publishes standards that affect various industries, including computing, ensuring compatibility and safety on a global scale.
		- International Electrical and Electronics Engineers (IEEE)
			- One of the larges organizations that set standards for electronic and electrical technologies.
			- It includes widely-used networking protocols like Ethernet (IEEE 802.3) and Wi-Fi (IEEE 801.11).
		- American National Standards Institute (ANSI)
			- Aligns US industry standards with global norms, ensuring that American products and companies remain competitive.
		- World Wide Web Consortium (W3C)
			- Establishes and maintains web standards like HTML, CSS, and XML.
			- Ensuring that the web functions uniformly across all browsers and platforms.
		- International Telecommunication Union (ITU)
			- This organization focuses on developing global standards for telecommunications.
			- Enruing that communication systems worldwide remain compatible and efficient.
		

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

- Diagram:
	![[CSP103-10.png]]
### Strengths of Standard Organizations
- Global Cooperation
	- Standard organizations encourage cooperation across countries and industries.
	- Ensuring that new technologies work globally.
- Product Compatibility
	- Standards ensure that devices, software, and systems from different manufacturers and regions can interoperate smoothly.
- Innovation and Competition
	- By providing a level playing field, standards encourage competition and innovation, enabling new technologies to emeger while maintaining interoperability.
- Compliance and Safety
	- Standards often enforce compliance with safety, security, and enviromental regulations, reducing risks for consumers and industries.
### Weakneses and Challenges
- While standard organizations have many strengths, they also face several challenges:
	- Slow Process
		- Consensus-based decision-making can slow down the creation of new standards, meaning that it can take years for new technologies to become standardized. 
	- High Compliance Costs
		- Adhering to standards can be costly for companies, especially small businesses, which may struggle with the expense of certifications, product redesign, or testing. 
	- Conflicting Regional Standards 
		- Sometimes, regional standards (e.g., European versus global standards) create conflicts, causing additional costs and complexities for manufacturers trying to meet all requirements. 
	- Resistance from Stakeholders
		- Some companies may resist adopting new standards, especially if it involves replacing or upgrading existing proprietary systems they've invested heavily in.
- Case Study: The Evolution of USB Standards
	- The USB (Universal Serial Bus) standard has evolved significantly since its inception in the mid-1990s. 
	- Initially, USB 1.0 allowed basic data transfer between devices, but it was quickly superseded by USB 2.0 with improved data transfer rates. 
	- As technology advanced, USB 3.0, 3.1, and 4.0 introduced even faster speeds and enhanced power delivery, making USB a versatile and essential standard in computing. 
	- Each iteration has maintained backward compatibility, allowing users to connect newer USB devices to older ports, illustrating the importance of maintaining compatibility while innovating.
	- Note:
		- Data Transfer Rates
			- Measured in Megabits per second (Mbps), or Gigabits per second (Gbps).
			- Higher versions offer faster file transfer speeds.
		- Connector Types
			- USB-A is the most common, but USB-C has become the industry standard for newer versions due to its reversible design and compatibility.
		- Power Delivery
			- USB standards support increasing power levels, with USB 3.1 or newer supporting up to 100W—making it ideal for charging larger devices like laptops.
		- Backwards Compatibility
			- USB versions are generally backwards compatible, meaning newer devices can work with older ports but at reduced speeds—depending on the generational gap between the two devices.

| Feature                    | USB 1.0/1.1                       | USB 2.0                                        | USB 3.0                                                | USB 3.1                                             | USB 3.2                                              | USB 4                                                                              |
| -------------------------- | --------------------------------- | ---------------------------------------------- | ------------------------------------------------------ | --------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------- |
| Release Year               | 1996 (1.0) / 1998 (1.1)           | 2000                                           | 2008                                                   | 2013                                                | 2017                                                 | 2019                                                                               |
| Maximum Data Transfer Rate | 12 Mbps (1.1)                     | 480 MBps                                       | 5 Gbps                                                 | 10 GBps                                             | 20 Gbps                                              | 40 Gbps                                                                            |
| Connector Types            | USB-A                             | USB-A, USB-B, Mini-USB, Micro-USB              | USB-A, USB-B, USB Micro-B, USB-C                       | USB-A, USB-C                                        | USB-A, USB-C                                         | USB-C                                                                              |
| Power Delivery             | 2.5W — 5V, 0.5A                   | 2.5W — 5V, 0.5A                                | 4.5W — 5V, 0.9A                                        | up to 100W, with USB Power Delivery                 | Up to 100W, with USB Power Delivery                  | Up to 100W, with USB Power Delivery                                                |
| Backwards Compatibility    | N/A                               | USB 1.X                                        | USB 2.0, USB 1.X                                       | USB 3.0, USB 2.0, USB 1.X                           | USB 3.1, USB 3.0, USB 2.0, USB 1.X                   | USB 3.X, USB 2.0, USB 1.X                                                          |
| Key Improvements           | Basic data transfer               | Higher speed, improved power delivery          | SuperSpeed data rates (5Gbps), better power efficiency | Enhanced data rates (10GBps), introduction of USB-C | Dual-lane operation for higher speeds, USB-c focused | Thunderbolt 3 support, higher speeds (40 Gbps), optimized for USB-C                |
| Use Case                   | Basic peripherals—mice, keyboards | Standard peripherals, external storage devices | High-speed data transfer, external storage             | Ultra high-speed transfer, video and data           | Fast data transfer, multiple devices, 4K video       | Ultra-fast data, external monitors, docking stations, and high performance devices |
- Diagram
		- ![[CSP103-11.png]]