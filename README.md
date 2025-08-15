# SRS-documentation
Documentation of Logirsim

# 1. Introduction
## 1.1 Purpose
The purpose of this document is to present a detailed description of the open-source
software Logisim. It will explain the purpose and features of the software, the interfaces of
the software, what the software will do and the constraints under which it must operate.
This document is intended for users of the software and potential developers.
## 1.2 Document Conventions
This Document was created based on the IEEE template for System Requirement
Specification Documents.
## 1.3 Intended Audience and Reading Suggestions
- Typical Users, such as engineering students who want to use Logisim to design
circuits for their class assignments, or circuit design enthusiasts
- Programmers, who are interested in creating a fork of the project, which they can
expand and personalize by adding features they need.
## 1.4 Product Scope
Logisim is a software for logic circuit simulation created by Dr. Carl Burch for educational
purposes. The software emphasizes simplicity of use has an intuitive user interface and it
includes many different circuit creation components, as well as useful tools for circuit
analysis.
## 1.5 References
Logisim’s website:
http://www.cburch.com/logisim/]
Logisim’s Library Reference:
http://www.cburch.com/logisim/docs/2.7/en/html/libs/index.html
Logisim on SourceForge:
https://sourceforge.net/projects/circuit/

# Software Requirements Specification for Logisim Page 2
IEEE Template for System Requirement Specification Documents:
https://goo.gl/nsUFwy
-Logisim: a graphical system for logical circuit design and simulation:
https://dl.acm.org/doi/10.1145/545197.545199

# 2. Overall Description
## 2.1 Product Perspective
Logisim is a software system for logic circuit design developed for educational purposes.
As educational software, it is widely used in many undergraduate programs around the
world. The applet offers a variety of logical components. Among others, Logisim includes
gates, multiplexers/demultiplexers, adders, multipliers, flip-flops, transistors, RAMs, clocks
and I/O. The straightforward user interface combined with the presence of the above
logical components, as well as it’s circuit analysis features, make Logisim a very powerful
educational tool.
It is an open source project that is currently inactive. Nonetheless, there are many forks of
the project whose development is very active.
## 2.2 Product Functions
Main Page
- Design Area: the area where the user can create or edit their own circuits.
- Top Menu: a typical top menu, with the following options: “File”, “Edit”, “Project”,
“Simulate”, “Window”, “Help”.
- Control options pane: a pane which contains some control toggles. For example,
these include a pointer that enables the user to edit the circuit, a way to change
values within the circuit, some basic circuit view toggles and more.
- Explorer pane: it can display project circuits and libraries, such as Wiring, Gates,
Plexers, Arithmetic, Input/Output and others. It can also serve as a way to view the
simulation hierarchy.
- Information pane: initially blank, it sits on the lower left of the window and it provides
information about the selected component.

# Software Requirements Specification for Logisim Page 3

## Top Menu
- File: this section hosts all the typical options for file manipulation, such as creating a
new circuit file, opening a saved circuit file, saving the current circuit file, exporting
the current circuit as an image and opening a Preferences panel.
- Edit: it includes many options for manipulating the components present in the
Design Area.
- Project: it allows the user to add circuits to the current project, load/unload libraries,
manipulating the appearance of the circuits and analyzing a circuit.
- Simulate: this section provides the user with options for simulating circuits.
- Window: this section allows the user to manipulate the size of the window
- Help: this section offers a tutorial, a guide, and an “About” section.
Design Area
This area is initially blank. The user can choose components from the Component
panel and add them to the Design Area.
Control options pane
- Link select (poke tool): it is used for changing the values within a circuit
- Normal select (edit/select tool): it is used for adding and editing components and
wiring.
- Text tool: it allows the user to add or edit text in circuits
- Shortcuts for logic components: this area of the panel includes some basic logic
components such as Pins (both East and West facing), NOT Gates, AND Gates,
OR Gates.
- Explorer pane view: it consists of two buttons which allow the user to choose what
they want the Explorer pane to show. The two options are a) Show project circuits
and libraries or, b) Show simulation hierarchy.
- Edit viewed circuit layout or circuit’s subcircuit appearance.

# Explorer pane
The Explorer pane consists of two different views:
Show project circuits and libraries:
- Any circuits added to the current project will appear there
- Wiring: Splitters, Pins, Probes, Tunnels, Pull Resistors, Clocks, Constants, Power,
Ground, Transistors, Transmission Gates, Bit Extenders
- Gates: NOT Gates, Buffers, AND Gates, OR Gates, NAND Gates, NOR Gates,
XOR Gates, XNOR Gates, Odd Parity, Even Parity, Controlled Buffers, Controlled
Inverters
- Plexers: Multiplexers, Demultiplexers, Decoders, Priority Encoders, Bit Selectors
- Arithmetic: Adders, Subtractors, Multipliers, Dividers, Negators, Comparators,
Shifters, Bit Adders, Bit Finders
- Memory: D Flip-Flops, T Flip-Flops, J-K Flip-flops, S-R Flip-Flops, Registers,
Counters, Shift Counters, Random Generators, RAMs, ROMs
- Input/Output: Buttons, Joysticks, Keyboards, LEDs, 7-Segment Displays, Hex Digit
Displays, LED Matrices, TTYs
- Base: Poke Tool, Edit Tool, Select Tool, Wiring Tool, Text Tool, Menu Tool, Labels
Show simulation hierarchy
This option shows the hierarchy of subcircuits being simulated.
Information pane
It consists of useful information and switches regarding a selected component. It
allows the user to view information about the component and change it.
## 2.3 User Classes and Characteristics
- Typical Users, such as engineering students who want to use Logisim to design
circuits for their class assignments, or circuit design enthusiasts
- Advanced Users, such as course instructors, who are experienced with using the
software.
- Programmers, who are interested in creating a fork of the project, which they can
expand and personalize by adding features they need.

## 2.4 Operating Environment
Logisim requires Java 5 or later. It runs under:
- Windows (.jar, .exe)
- MacOS X (.jar, .tar.gz)
- Linux (.jar)
## 2.5 Design and Implementation Constraints
Logisim was developed in Java. It is very lightweight and it does not rely on any software
tools or applications.
## 2.6 User Documentation

There is a tutorial, a user guide and a library reference for each version -starting with 2.1.x-
on Logisim’s website:

http://www.cburch.com/logisim/docs.html
Additional information about Logisim can be found on SourceForge:
https://sourceforge.net/projects/circuit/
There is a subreddit dedicated to Logisim that is very active:
https://www.reddit.com/r/logisim/
Also, below is a link to a YouTube tutorial on Logisim, covering basic features:
https://www.youtube.com/watch?v=cMz7wyY_PxE
## 2.7 Assumptions and Dependencies
Logisim can run on pretty much any computer running Java version 5 or later. Specifically
on Windows, the user can run the software either by downloading the .jar file or the .exe
file. Alternatively, they could use an open-source tool such as launch4j to wrap the Java
application file in a Windows executable.
