# LRU
This is a simple Least-Recently used Cache implemented in Java 1.6.0


# General Readme

Hello! Thank you so much for getting me this far in the application process, and I also loved the interview problem, fun times :) 

## Versions

The initial push aptly named **"The First and Finial"** and [accessible via this link](https://github.com/funkeyfreak/LRU/commit/e87e44a2c7d3afc7cfb224ea0751996e0905dfcc) is the code developed within the 2 hour limit. I have not added the JUnit framework because I kept 'tabs' of my stubbed tests in an atom.io text file. The second push shall be added shortly, detailing all the unit tests I have written!

## Basic Instructions

The layout and general instructions can be seen per the instruction file sent to be (if you do not have this file, why are you here?!).  The set of commands are case sensitive, so be advised. The commands function as follows:

* SIZE : This command initializes the size of the LRU cache. This command **MUST** be ran first, and can only be ran once. EXAMPLE: SIZE 5.
* SET : This command sets a key k to some value v within our cache. EXAMPLE SET k v. NOTE, if the key exists, this command WILL overwrite it.
* GET : This command gets the value associated with the key provided. If no key exists, we get an NOTFOUND message. EXAMPLE GET k.
* EXIT : This command exists the application. EXAMPLE EXIT.

## Installation Instructions

Being a petty windows user (for the time being), I used IntelliJ IDEA (the bulk of the developing) and eclipse (for testing the project in Java 16) for my development process, and therefore used that terminal for running my application. I have also followed the instructions [here](https://docs.oracle.com/javase/tutorial/getStarted/cupojava/win32.html) to run the application from cmd prompt. The cmd used in **java -cp . LRU** ran from within the .\LRU\bin folder. This will initialize your application and allow you to run as many tests as you would like.

As for Linux, I did not have a VM on hand given I was not at my desktop, so unfortunately I do not have precise instructions for Linux

## Assumptions 

1. I assumed the user would be mindful of their capitalization during cmd usage.
2. I assumed the user would at least have a decent understanding of how threading works and would not use this within such an environment without changing several key race conditions.
3. Seeing how I have not tried every available input variation, I assumed the strings tested were suffice.
4. I assumed if the user did not pass a valid integer, they wanted a LRU cache of size 64! Oh golly!

## Issues and Limitations

I ran into several issues after my first iteration, where I took a plan linked list and attempted to implement this algorithm. After a bit of refactoring, I arrived at the solution as you see it! If there are any errors found, please create a pull request and keep this code snazzy :smiley:.
