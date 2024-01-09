# `git`, the SDLC, and TDD -- oh my!

In this initial "pseudo-ish" :-) programming assignment, you'll practice debugging, test driven-development (TDD), and generally familiarize yourself in working with git and the terminal. I strongly recommend starting on this early in the event that you encounter process related issues -- such as commiting and/or pushing your work. Give yourself time to reach out to me or one of the course LAs/IAs/TAs.

## Part 1: Test Driven Development (TDD)

In this first part you'll practice: running tests, writing tests, identifying bugs using tests, and implementing bug fixes. 

First, `cd` into the directory where you are storing your work for 311 this semester, clone this repo, then open the cloned repo in IntelliJ. 

> If you want a video walkthrough of me doing this on a sample repo, check the Lesson notes regarding use of the terminal and git under Module 02 on canvas. And/or consult the media gallery on canvas -- which contains a recording.

### Code Specification:

We are solving a classic interview problem, finding the longest prefix in an ArrayList of Strings. These types of problems feature heavily in interviews, and String manipulation in general is a very routine practice that you as a developer should be familiar with. Here is the problem statement for the longest common prefix problem:

> You must find the longest common prefix in an array of Strings. If there is no common prefix, return an empty string (i.e. ""). If there is a common prefix, return it as a String

#### Some examples:

- in this array ["flower", "flow", "flight"], we would return "fl" as the longest common prefix
- in this array ["flower", "flow"], we would return "flow"
- ["dog", "racecar", "car"], we would return ""
- in this array [], we would return "" as there are no strings at all

### Step 0: adding dependencies of `jUnit`

Rather than using the version of jUnit packaged with IntelliJ (as we did with a prior activity), the starter kit for this repo includes a **maven** `pom.xml` in the root directory of your cloned repo. 

This is an example of *build script* -- in developers can define how executables for their project's get built, as well as libraries and dependencies that their project might depend on. A simple, well written build scripts is nice, durable way of handling and managing codebases long term (especially those that rely on many different libraries -- 99% of which won't be packaged with in IntelliJ). 

There are many different types of build tools out there for Java (some more complicated than others -- e.g., **gradle**.. *my 2cents only..*). Maven is pretty much the de-facto standard. 

First: you'll need to add a dependency to minimal `pom.xml` included in the starter kit. First go to the maven (mvn) central repo [here]().



### Step 1: review the existing prefix-finding code

In the blue `src` folder in the starter kit for this repo, you'll find an existing solution and some test cases (in the green folder marked `test`). 
