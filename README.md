# Network-Flow-Analyzer
This project will be carried out under the supervision of my professor Mirko Puliafito, lecturer of the networking course I'm currently following in university, and 
also the founder and the CEO of Digitiamo SRL.

https://en.digitiamo.com/                   
https://www.uninsubria.it/ugov/degreecourse/175326           

# Project description
This project consists in an application that analyzes network traffic, by taking raw packets and categorizing them (e.g: video streaming flows, messaging flows, etc.).   
The analysis starts by sniffing the traffic on a network. Each information will be stored in a centralized database, where each block of information indicates what user produced what kind of information at a given time.                      
A statistical analysis follows, so that a data model containing the occurrencies of the various traffic types is produced.   
Other activities will rely on the model, such as defining constraints (e.g: limiting streaming activities to 10 GB), or forecasting attacks.   
The project is a long-term one, so it'll gradually evolve.   

# Programming language
The chosen programming language is C++ for the following reasons:   
- memory management: the application will handle hundreds to thounsands packets at once, therefore the memory better be handled manually, in order to avoid performance issues or memory problems such as memory leaks;
- rawer approach: one of the main reason this project was born is to challenge myself, so I wanted to spice it up a little by using a language that has trickier features;
- natively oop: c++ has been conceived as an oop language, so it consequently has oop features such as visibility, classes, polymorphism, etc. On the other hand, there's Python, which is a simpler language with plenty of libraries, but it is a little too simplified for my purposes and it implements the oop paradigm poorly (e.g: Python doesn't handle visibility).
- faster: as stated above, memory can be managed manually and hence there is the possibility of choosing to either use dynamic memory or static memory.

# Library used
PcapPlusPlus will be used in this project.

# Steps
- Sep 1: build a basic network sniffer and categorize the data in a local database.
