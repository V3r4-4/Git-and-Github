# Introduction to Version Control Systems

Version Control System is a software the tracks Source code changes and manages the code.

# A simple example of how the system development cycle works

    -A school library needs a digital library services system for learners to access E-books, To renew borrowed books remotely and to check out the library catalogue. The school management system approaches a Software Development Company, they get to an agreement and the company is given five days to present a prototype of how the system will look like.
    -The Company presents the prototype and the school management likes it. They agree that payments will be done per milestones (ie 20% for front-end completion). The company is given a deadline. Immediately, the company plans the development process.
    -The development team is given the resources needed. System analyst and project Manager assigns tasks to teams(e.g Software engineers, Database schema, Back-end developers e.t.c). They choose how the project will be managed whether it is through Monorepo(Whole application in one Repository) or Micro-services(An application divided into multiple parts which are stored in multiple repositories). How the application runs monolithic(One big running application) or micro-services(Many small services communicating via a network). And after planning, the development process begins.
    -Each developer and programmer is given a task. Let's consider how the front-end team manages their code if the project was to run through micro-services. 
        -Developer A is working on HTML and CSS.
        -Developer B is working on JavaScript.
        -Both developers will pull the Front-end Repository to their computers.
        -Developer A creates his part  in their branch.
        -Developer B also creates his part in their branch.
        -Once done they submit a pull request and Team Lead checks if it meets security standards. Team Lead approves both their works and merges both branches to the main branch.
        -The front-end is now complete. They test it. They find it works, they show it to client and receives 20% of full amount.


#### Problems developers faced that led to development of Version Control Systems?

* Saved their work in their local computers, which meant that if the computer was damaged the all changes and project was gone.
* Manually created a copy of a file every time they made a change. The problem was the confusion they went through to identify which file version had specific change, What changes were made and who made them and at what time. This made the development process even slower.
* Developers could overwrite each each others work. The developers passed the work they've worked on to other teammates using a floppy disk/CD.
* The team Lead reviewed code either print out on paper or they had to walk to the developers work station to review their work.

<br>
<br>
<br>

#### How Version Control Systems solved the problems.

* Developers overwriting each others work - Two developers edited the same work on the drive. Version control system like git enabled each developer to have their own branch. During merging if there's any overwriting git highlights a conflict.
* Nobody knew which folder contained the real working code. Cause remember a developer could take a file containing code, copy it, make a change and then save the file with a name to show which version it is. - Version control systems like git Repository hosts main branch that is clear and other separate branches  for experimental features.
* Loss of history. Incase of a bug, nobody knew who wrote the code, who made the changes and why they made it.
Git has git log/git blame which point out to the author-who made the change, timestamps-the time the change was made- and has commit message to show what changes were made.
* Incase a developer made a mistake or tried out an experiment which led to losing the working project- It was difficult or rather impossible to reverse the working directory. In git, there git revert/git reset which helps restore the original working project.
* Backing up a project in case the server crashed, In both local and centralized if the local computer or the server went down then the whole project got lost. But by using git, once the developer has cloned the whole project to their computers they don't lose it. In short, every developer or member of the team has a copy of the main project hence enough backup.
* For code reviews where team leads had to review a developers code and to find changes, the team lead back then has to read thousands of lines of code to see changes. In git, It highlights changes made, If deletion was made it is highlighted in red and if something was added, it is highlighted in green.
<br>
<br>
<br>

# Evolution of Version Control Systems.
<br>

#### Local Version Control System
        - There was a database in a single machine(computer) that tracked any changes made to files in that machine.
        - It showed differences in the files(previous version and current version)
        - Disadvantage: It was impossible to collaborate, and in case of damage of the machine, the whole project was lost.

<br>
<br>

#### Centralized Version Control System
        - There is a server that stores all different versions of the file and the changes made. Every time someone made a change to a file, they commit the changes to a central server.
        - It showed different versions of the file.
        - Incase of failure of the server all changes, files and project got lost.
<br>
<br>

#### Distributed Version Control System
        - In distributed Version Control Systems, the project, commits and changes are stored in each team member's computer as well the server. - It's a combination of both local and centralized version control. This is because the project, commits and history are stored in the server and the local computer of the developer so in case of crashing of either of them, There is backup of the project.
        - Each Developer gets to work on their own branch and later on the branches are merged.
<br>
<br>
 
# Version Control Systems created in the past before git and GitHub
<br>

#### Source Code Control System (SCCS)
    - It's a local Version Control System
    - It was created in Bell Labs
    - It ran on a single machine and tracked changes to individual files by storing original files and "deltas" differences.
    - Replaced manually renaming backing up files and allowed developers to revert an individual file to an earlier date. MEANING: When we mentioned that every time developers made changes  to a file, they copied the previous files then made changes to one of the files.
 <br>
 <br>
 
#### Apache Subversion(SVN)
    -It is a centralized VCS
    -It commit the entire directory as a/in a single commit in the  central server.
 <br>
 <br>
 
#### Concurrent Version Control(CVC) - Multiple people would make multiple changes to one file
<br>
<br>

#### Bitkeeper- It inspired the creation of git. Git works same as Bitkeeper.
<br>
<br>
