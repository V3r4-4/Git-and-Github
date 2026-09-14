# What is a Version Control System?

Version Control System is a software the tracks Source code changes and manages the code.

# A simple example of how the system development cycle works and where we need the Version Control Systems

    A school library needs a digital system so students can access e-books, renew borrowed books remotely, and search the library catalog. School management reaches out to a software development company, and they agree on a deal: the company gets five days to present a working prototype.

    The company presents the prototype, and the school loves it. They set a deadline and agree on milestone-based payments (like 20% upon front-end completion). The company kicks off planning immediately.

    The development team gets their resources, while the system analyst and project manager assign tasks to team members (software engineers, back-end developers, database engineers, etc.). They decide on the project setup—choosing between a single repository or multiple repositories for code storage, and a monolithic or microservices setup for the app architecture.

    Once planning wraps up, coding begins:

    Developer A builds the library catalog search interface.

    Developer B builds the book renewal dashboard.

    Both developers pull the front-end repository to their local machines.

    Developer A works on his component in a feature branch.

    Developer B works on his component in a separate feature branch.

    When finished, both submit pull requests. The team lead reviews the code for security and quality, runs tests, approves the work, and merges both branches into the main branch.

    The front-end phase is finished! After a quick client demo, the company collects their 20% milestone payment.

# Problems faced by developers

* Creating multiple versions of the project (e.g Front-end_v1, front-end_v2) to track changes. This caused confusion among developers trying to find out who made a change to a file, what change was made and why the change was made.
* During use of local version control systems, developers stored and tracked changes to source code in one local computer, which meant if the computer was damaged the all changes and project was gone.
* Team Lead reviewed code on paper or by going to each developer's workstation.
* In reviewing code, Team Lead had to go through thousands lines of code to spot changes. 
* Developers would make similar changes to same file ie overwriting each others work.
* The developers passed the work they've worked on to other teammates using a floppy disk/CD.
* Team Lead reviewed code printed out on paper or had to walk to the developer's workstation to review their work.

<br>
<br>
<br>

# How Version Control Systems solved the problems.
* To solve the problems developers faced, severall Version Control Systems were created. Here are some ot the systems and how they worked to solve the problems:
* <br>


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

* 
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


