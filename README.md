## Version Controlling System (VCS):
Source Code Repository:
  - Features:
    - Distribution
    - Tracking File History
    - Disk Space
    - Security

### Working:
  - Remote Repository
      - GitHub
      - GitLab
      - BitBucket
      - AWS Code Commit
      - Azure repo
  - Development Env:
      - Git Software (Git Bash)
      - MobaXterm
      - Editor (Atom / VS / PyCharm)
      - VirtualBox
      - Vagrant

### Development Env:
  $ git version

### Git Settings:
  - Define User name
    - $ git config --global --list
    - $ git config --global user.name "rnstech"
  - Define Email ID
    - $ git config --global user.email "rnstech@gmail.com"
    - $ git config --global --list

### Remote Repo:
  - Sign Up GitHub
  - Sign in to GitHub
  - Create New Repository in the GitHub - 'DockerComposeProject'

### Go to Windows System:
  - Install 'Git Bash' on windows
  - Choose the directory 'E:\workspace\batch54'
  - git clone https://github.com/accountid/DockerComposeProject.git
  - go to 'DockerComposeProject' (cd DockerComposeProject)
  - Open in VSC Editor
  - Craete all the Project files
  - Then push to Remote Repo

#### Git Work Flow:
  - Workspace --> Staging (add) --> Local Repo (commit) --> Remote Repo (push)

    $ git pull origin master

    $ ls -l

    $ git status

    $ git add Dockerfile README2.md

    $ git status

    $ git add .

    $ git status

    $ git commit -m "Docker Compose project initial files created"

    $ git status

    $ git push origin master

      - GutHUb UN: venkat09docs
      - 
      - GitHub Key: 
      - 
        (Goto GitHub --> Profile Icon --> Settings --> Developer Settings --> Personal access tokens (classic))
        
#### Git Merge Conflicts

    $ git push origin master

    $ git pull origin master

    $ git mergetool

    $ ls -l

    $ cat Dockerfile

    $ ll

    $ rm Dockerfile.orig

    $ git status

    $ git commit -m "Conflict resolved"

    $ git push origin master

### Branching Directories:
    - Development Branch
      - Feature Branch
    - Release Branch  
    - Master / main branch (Prod)
    - Tagging on master branch

### Branching Activities:

  1. Creating Branch
      - master --> dev
      - dev --> feature2
      - dev --> feature1
      - dev --> release1
  
    - Formula:
      - src --> dest
      - $ git checkout src_branch
        $ git branch dest
  
  2. Committing to the specific Branch
      - commit files to feature2 branch
      - commit files to dev branch
      - commit files to feature1 branch
      - commit files to release1 branch (bug fixes)

    - Formula:
    - $ git checkout branch
    - $ git commit -m "msg"
    - $ git push origin branch
  
  3. Merging Branches
      Ex: 
        feature1 -> dev
        release1 -> master
        release1 -> dev

    - Formula:
      - src --> dest
      - $ git checkout dest
      - $ git merge src_branch
      - $ git push origin dest

  4. Tagging the release branch (master)
      Ex: master branch

    - Formula
      $ git checkout master
      $ git tag tag_name
      $ git push origin tag_name

  5. Deleting temporary branches
      Ex: feature1

      $ git branch -d feature1
      $ git push origin :refs/heads/feature1


## How you can build this project

Step-1: Run the following command

    $ docker-compose up

Step-2: Enter http://IPAddress:8000/ in a browser to see the application running.

Step-3: Terminate the Application

    $ docker-compose down
