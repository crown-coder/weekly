**Git Demo Project**
Overview
This project demonstrates the use of Git commands in a real-world workflow. 
It includes a simple HTML webpage with features like a navbar and footer, 
developed using Git branching, merging, and other advanced commands. 
The workflow simulates a collaborative development process.

**Features**
Initial project setup and Git repository creation.
Branching for feature development (feature/navbar, feature/footer).
Merging branches into the main branch.
Conflict resolution during merges.
Advanced Git commands:
Stashing changes.
Tagging releases.

**Git Workflow**

1. Project Initialization
mkdir git-demo-project
cd git-demo-project
git init
Created the repository and added a remote connection.

2. Branching and Feature Development
Create a New Branch

git checkout -b feature/navbar
Add Changes
Modified index.html to include a navbar:

<nav>
    <div class="logo">
      <h1>CrownCoder</h1>
    </div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
   </nav>
   
Commit and Push Changes

git add index.html
git commit -m "Added navbar"
git push origin feature/navbar
3. Merging Branches

Switch back to main and merge:

git checkout main
git merge feature/navbar
git push origin main

4. Handling Merge Conflicts
Simulated a conflict by editing index.html in main and feature/footer. 
Resolved the conflict manually and committed the changes:

git add index.html
git commit -m "Resolved merge conflict for footer"
git push origin main

5. Advanced Commands
Stashing Changes
Saved uncommitted changes temporarily:

git stash
git stash list
git stash apply
Tagging a Release
Tagged the first release:

git tag -a v1.0 -m "First release"
git push origin v1.0
How to Run the Project

Clone the repository:

git clone https://github.com/crown-coder/weekly.git
Open index.html in a browser to view the project.
Key Git Commands Used

**Command	Purpose**
git init	Initializes a new Git repository.
git add	Stages changes for the next commit.
git commit	Saves changes with a descriptive message.
git branch	Creates and lists branches.
git checkout	Switches to a different branch.
git merge	Merges changes from one branch into another.
git push	Pushes changes to a remote repository.
git stash	Temporarily saves changes that aren’t ready to commit.
git tag	Marks a specific commit as a release version.
git log	Displays commit history.
Project Demo
Visit the live demo on GitHub Pages or view the repository on GitHub.

