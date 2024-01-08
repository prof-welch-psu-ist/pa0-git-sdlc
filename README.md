# `git`, the SDLC, and TDD

In this initial (half! :-) programming assignment, you'll practice debugging, test driven-development (TDD), and generally familiarize yourself in working with git and the terminal. I recommend starting early on this in the event that you encounter process related issues -- such as commiting and pushing your work.

## Part 1: Test Driven Development (TDD)

In this first part, you'll practice: running tests, writing tests, identifying bugs using tests, and implementing bug fixes. 

First, `cd` into the directory where you are storing your work for 311 this semester, clone this repo, then open the cloned repo in IntelliJ. 

> If you want a video walkthrough of me doing this, check the Lesson notes regarding use of the terminal and git under Module 02 on canvas and/or consult the media gallery on canvas (which contains a recording where I give a sample).

### Code Specification:

We are solving a classic interview problem, finding the longest prefix in an ArrayList of Strings. These types of problems feature heavily in interviews, and String manipulation is a common practice that you will need to master to be an effective developer. Here is the problem statement:

> You must find the longest common prefix in an array of Strings. If there is no common prefix, return an empty string (i.e. ""). If there is a common prefix, return it as a String:

#### Some examples:

- in this array ["flower", "flow", "flight"], we would return "fl" as the longest common prefix
- in this array ["flower", "flow"], we would return "flow"
- ["dog", "racecar", "car"], we would return ""
- in this array [], we would return "" as there are no strings at all

### Step 0: adding dependencies of `jUnit`

Rather than using the version of jUnit packaged with IntelliJ, the starter kit for this repo includes a **maven** `pom.xml` in the root directory of your cloned repo. This is an example of *build script* -- in which developers add external libraries and dependencies to their projects. 

There are many different types of build tools out there (some more complicated than others -- e.g., **gradle**.. *my 2cents only..*). The section of the `pom` that 
### Step 1: review the existing code

In the blue `src` folder in the starter kit for this repo, you'll find an existing solution and some test cases for the longest common prefix method provided. 
