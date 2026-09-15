# What is a Version Control System?
A Version Control System (VCS) is software that tracks and manages changes to your source code over time. It allows developers to keep a complete history of their work, undo mistakes, and collaborate safely on the same project without overwriting each other's code.
<BR>

### What happens with and without version control systems?
<BR>`
A school library hires a tech company to build a website where students can search for books and renew them online.
Developer A and Developer B start working on the project at the same time:

* **Without Version Control:** Both developers work on the same file at the same time. Developer A writes code for the search bar. Developer B writes code for the renewal page. When Developer B saves his file, he accidentally deletes Developer A's search bar code. Because there is no saved history, Developer A's work is lost completely.

* **With Version Control (VCS):** Both developers work on their own separate copy of the project. When they finish, the VCS automatically compares their files. It combines both updates into the main project without deleting anyone's work. If a mistake happens, the team can easily go back to an older, working version of the website.
<BR>
<BR>

### Why do Version Control Systems Exist?
<BR>
Before Version Control Systems (VCS), software development teams faced major challenges:

* **Messy File Naming**: Developers created multiple project folders to track updates (for example, Front-end_v1, Front-end_v2). This made it hard to know who made a change, what was changed, or why.

* **Risk of Total Data Loss**: Early local tracking systems kept all files on a single computer. If that computer broke, the entire project and its history were permanently lost.

* **Painful File Sharing**: Developers shared their code with teammates using floppy disks, CDs, or email.

* **Accidental Overwrites**: Multiple developers often edited the same file at the same time, leading to workers accidentally deleting each other's code.

* **Inefficient Code Reviews**: Team leads had to review changes by printing out thousands of lines of code on paper or physically walking to each developer's desk.
<BR>
<BR>

### How Version Control Systems Solved These Problems?
<BR>
Version control systems evolved through three main stages:

* **Local VCS (Example: SCCS)**
    - Instead of manually copying folders like Front-end_v1 and Front-end_v2, local systems automatically tracked changes to individual files on a single computer. Developers could easily go back to an earlier version of any file if they made a mistake.
* **Centralized VCS (Example: Subversion / SVN)**
    - To stop developers from passing code on physical CDs or floppy disks, centralized systems stored all files on a main server. Developers could download files from the server and upload their updates. However, if the main server crashed, nobody could work.
* **Distributed VCS (Example: Git)**
    - Modern tools like Git solved the server crash problem. Every developer gets a full copy of the entire project history on their own computer. If the server goes offline, no work is lost. Git also allows multiple people to work on feature branches at the same time and safely merge their code without overwriting each other's work.

### Git and GitHub: What Is the Difference?
Because Git and GitHub are used together, many beginners think they are the same tool. However, they serve two different purposes:

* **Git (The Tool)**
    - Git is the actual software installed on your computer. It tracks changes in your code, manages your project history, and lets you work on separate branches locally without needing an internet connection.

* **GitHub (The Service)**
    - GitHub is a cloud-based platform that hosts your Git repositories online. It allows team members to share their code, review each other's work through Pull Requests, and collaborate from anywhere in the world.
<BR>

**Simple Analogy: Think of Git like video editing software on your laptop, and GitHub like YouTube where you upload and share your videos with others.**
