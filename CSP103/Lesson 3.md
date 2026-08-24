### > [Table of Contents](../main.md)
# CSP103
---
## Target
- Learning Outcomes
	* Explain the importance of standards in computing and their role in ensuring interoperability, consistency, and innovation.
	- Identify key computer organization standards and describe their impact on the development and compatibility of computer systems.
- Topics
	4. Introduction to Standard Organizations
	    + 4.1. Importance of Standards in Computing
	    + 4.2. Computer Organization Standards
	    + 4.3. Strengths of Standard Organizations
	    + 4.4. Weaknesses and Challenges
## __Introduction to Standard Organizations__
- Background:
	- Standard organizations in computing play a pivotal role in ensuring that technologies across different platforms can communicate, integrate, and evolve cohesively.
	- These organizations set the groundwork by defining protocols, guidelines, and specifications that fosther interoperability, enhance safety, and streamline global technological advancements.
### __Importance of Standards in Computing__
- Definition:
	- __Standards are essential__ for creating a harmonized digital ecosystem. They lay the __foundation for cooperation between hardware and software systems__, ensuring they __work together efficiently__.
- Key areas:
	- __Interoperability__
		- Standards ensure that __different devices, software, and systems can communicate and work together seemlessly__.
		- For instance, the _TCP/IP_ protocol __enables consistent internet functionality__ worldwide.
	- __Quality and Safety__
		- Standards __benchmark product performance and safety__.
		- For example, _cybersecurity_ standards ensure that products meet specific criteria to __protect users from cyber threats and safety__.
	- __Facilitation Innovation__
		- Standards __establish clear frameworks for development__, enabling innovators to create technologies that __work harmoniously with existing systems__.
	- __Compatibility__
		- Standards ensure both __backward and forward compatibility__, maintaining the utility of older technologies.
		- For instance, devices using USB 3.0 are still often compatible with USB 2.0 ports.
### __Computer Organization Standards__
- Definition:
	- Several types of standards __governs a computer system's key components and operations__ within a computer organization.
	- These standards are __critical for ensuring that all components communicate efficiently and operate reliably__.
- Categories of Standards in Computer Organization:
	- __Bus Standards__
		- Definition:
			- Buses are the __communication pathways that transfer data__ between computer components.
			- The bus standards __define how components__ like the CPU, memory, I/O devices and other peripherals __communicate__.
		- Common Bus Standards:
			- __Peripheral Component Interconnect__ (_PCI_)
				- A standard for __connecting peripheral devices__.
			- __Peripheral Component Interconnect Express__ (_PCIe_)
				- An advanced version of _PCI_, offering __faster data transfer rates__.
			- __Universal Serial Bus__ (_USB_)
				- A __standard for connecting external devices__, such as keyboards, printers, and storage devices.
		- Example:
			- PCIe is a high-speed bus standard widely used in modern computers to connect the CPU, with high-performance components like graphics cards, SSDs, and network cards.
	- __Memory Standards__
		- Definition:
			- Memory __standards ensure that memory devices__—such as RAM, __work effectively__ with other system components.
			- It defines everything from physical dimensions to electrical characteristics, speeds, and capacities.
		- Common Memory Standards:
			- _DDR4/DDR5_
				- Stands for __Double Data Rates__.
				- High-speed RAM standards __used in most modern computers__.
			- _SDRAM_
				- Stands for __Synchronous Dynamic Random Access Memory__.
				- Used in __older data storage and management systems__.
			- _ECC Memory_
				- Stands for __Error-Correcting Code Memory__.
				- A specialized memory standard used in servers for __detecting and correcting memory errors__.
		- Example:
			- _DDR_ standards govern how RAM modules communicate with the CPU.
			- Current standards include DDR4 and DDR5, which differ in data transfer rates and power consumption.
		- Diagram:
			![[CSP103-8.png]]
	- __Display Standards__
		- Definition:
			- Governs how __computers transmit visual data to monitors__ and other output devices.
			- These standards __ensure that the display output is consistent__, regardless of the manufacturer and device type.
		- Common Display Standards:
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
		- Example: _HDMI_ is a widely used standard for transmitting high-definition video and audio signals between computers, TVs, and monitors.
		- Diagram:
			![[CSP103-9.png]]
	- __Networking Standards__
		- Definition:
			- Networking standards dictate __how data is transmitted across networks__, whether __locally__ (e.g., a home network) or __globally__ (e.g., the internet). 
			- These standards __enable various devices to communicate__ over wired or wireless networks.
		- Common Networking Standards:
			- __Ethernet__ (_IEEE 802.3_)
				- A standard for __wired LAN communication__.
			- __Wi-Fi__ (_IEEE 801.11_)
				- Short for __Wireless Fidelity__.
				- Standards for __wireless network communications__.
			- __Bluetooth__
				- A wireless communication standard for __short-range data exchange__.
			- Example: _IEEE 802.11_ defines the standards for wireless communication, commonly known as _Wi-Fi_. Different versions, like _802.11n_ and _802.11ac_, provide different data transfer speeds and ranges.
- Main Organization Standards:
	- Background:
		- Various organizations oversee the development of these computing standards.
	- Some of the significant standard organizations include:
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
- While standard organizations have many strengths, they also face several challenges:
	- __Slow Process__
		- Consensus-based decision-making can slow down the creation of new standards, meaning that it can take years for new technologies to become standardized. 
	- __High Compliance Costs__
		- Adhering to standards can be costly for companies, especially small businesses, which may struggle with the expense of certifications, product redesign, or testing. 
	- __Conflicting Regional Standards__
		- Sometimes, regional standards (e.g., European versus global standards) create conflicts, causing additional costs and complexities for manufacturers trying to meet all requirements. 
	- __Resistance from Stakeholders__
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

# > [Lesson 4](/CSP103/Lesson%204.md)