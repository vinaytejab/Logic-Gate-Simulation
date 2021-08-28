# Github Page URL:
   (https://vinaytejab.github.io/Logic-Gate-Simulation/Main%20file/Codes/simulation.html)

# Documentation For Project(DLD-Comparator)

### Comparator -Introduction

A magnitude digital Comparator is a combinational circuit that compares two digital or binary numbers in order to find out whether one binary number is equal, less than or greater than the other binary number. We logically design a circuit for which we will have two inputs one for A and other for B and have three output terminals, one for A > B condition, one for A = B condition and one for A < B condition.

###### Figure

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic.png)

## This project is a simulation of the comparators made in Digital Logic Design(DLD). It has only 2-Bit Comparator currently inbuild in the project which can be use for user reference .

### 1-Bit Magnitude Comparator:

A comparator used to compare two bits is called a single bit comparator. It consists of two inputs each for two single bit numbers and three outputs to generate less than, equal to and greater than between two binary numbers.

The truth table for a 1-bit comparator is given below:

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic3.png)

#### From the above truth table logical expressions for each output can be expressed as follows:

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic1.png)

#### From the above truth table logical expressions for each output can be expressed as follows:

A>B: AB'
A<B: A'B
A=B: A'B' + AB

#### From the above expressions we can derive the following formula:

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic2.png)

#### By using these Boolean expressions, we can implement a logic circuit for this comparator as given below:

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic3.png)


### 2-Bit Magnitude Comparator :

A comparator used to compare two binary numbers each of two bits is called a 2-bit Magnitude comparator. It consists of four inputs and three outputs to generate less than, equal to and greater than between two binary numbers.

#### The truth table for a 2-bit comparator is given below:

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic4.png)

#### From the above truth table K-map for each output can be drawn as follows:

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic5.png)

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic6.png)

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic7.png)

#### From the above K-maps logical expressions for each output can be expressed as follows:

A>B:A1B1’ + A0B1’B0’ + A1A0B0’

A=B: A1’A0’B1’B0’ + A1’A0B1’B0 + A1A0B1B0 + A1A0’B1B0’

   : A1’B1’ (A0’B0’ + A0B0) + A1B1 (A0B0 + A0’B0’)
   
   : (A0B0 + A0’B0’) (A1B1 + A1’B1’)
   
   : (A0 Ex-Nor B0) (A1 Ex-Nor B1)
   
A<B:A1’B1 + A0’B1B0 + A1’A0’B0

#### By using these Boolean expressions, we can implement a logic circuit for this comparator as given below:

![Image](http://cse15-iiith.vlabs.ac.in/images/comp1.png)

### Cascading Comparator:

A comparator performing the comparison operation to more than four bits by cascading two or more 4-bit comparators is called cascading comparator. When two comparators are to be cascaded, the outputs of the lower-order comparator are connected to corresponding inputs of the higher-order comparator.

![Image](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Digitallogic11.png)

### Applications of Comparators :

1. Comparators are used in central processing units (CPUs) and microcontrollers (MCUs).
2. These are used in control applications in which the binary numbers representing physical variables such as temperature,       position, etc. are compared with a reference value.
3. Comparators are also used as process controllers and for Servo motor control.
4. Used in password verification and biometric applications.

## Objective:

1. The objective of this experiment is to understand working of the comparator.
2. Try to make 2-bit comparator.

## Procedure:

1. With The help of Theory Page , try to build the Comparator Circuit.
2. First of all build the basic 2-bit comparator .
3. If You are unable to make it , load the circuit directly and use it.
4. If want to see the circuit which you have stored in your system then load it first and continue it make changes to it.
5. Use the SAVE button to save it in your system for furture reference.

# Technical Details:

## Languages Used:
1. HTML
2. CSS
3. Javascript

## Libraries Used:
1. [Bootstrap](https://getbootstrap.com/) 
2. [jQuery](https://jquery.com/)

## Module Used
1. [Simcir](https://kazuhikoarase.github.io/simcirjs/)
[github link](https://github.com/kazuhikoarase/simcirjs)

## Implementation:

### The simcir module

The simcir module basically searches for a div with class named "simcir". It reads the json data inside that div, and transforms it into a live simulation. 

The json data contains the following things:
1. width(integer)- width of the simulator on the screen in px
2. height(integer)- height of the simulator in px
3. showToolbox(boolean)- decides if the toolbox(the left panel) is to be displayed or not.
4. toolbox(array)- items/tools to be shown in toolbox
5. devices(array)- devices to be displayed on the breadboard
6. connectors(array)- connections between the simulated tools/items.

## Test Cases

### Test Case 1

#### Clear Workspace

Input: click
Output: page refresh with blank breadboard and interaction enabled(with settings intact). 

Test case passed.

### Test Case 2

#### Help

Input: click
Output: Takes to to help view in a different page.

Test case passed.

### Test Case 3

#### Get Circuit Data

Input: click
Output:Shows the circuit data in the text box.

Test case passed.

### Test Case 4

#### Load Circuit Data

Input: click
Output:Inpuits the circuit data from textbox as simulation in the grid.

Test case passed.

### Test Case 5

#### Save Circuit Data

Input: click
Output:Saves the circuit data after a file name is given into the system.

Test case passed.

### Test Case 6

#### Load File

Input: click
Output: loads the choosen file into the text box.

Test case passed.

### Test Case 7

#### Clear Circuit Data Box(text box)

Input: click
Output:Clears the textbox.

Test case passed.

### Test Case 8

#### Load 2-bit Comparator

Input: click
Output:Loads the 2-bit comparator into the Simulation place.

Test case passed.

### Test Case 9

#### Simulation

Input: drag/drop/connections
Output: everything working correctly. 

Test case passed.
