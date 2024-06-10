## Version Controlling System (VCS):
Source Code
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

    git pull origin master
    ls -l
    git status
    git add Dockerfile README2.md
    git status
    git add .
    git status
    git commit -m "Docker Compose project initial files created"
    git status
    git push origin master
      - GutHUb UN: venkat09docs
      - GitHub Key: 
        (Goto GitHub --> Profile Icon --> Settings --> Developer Settings --> Personal access tokens (classic))
        

## How you can build this project

Step-1: Run the following command

    $ docker-compose up

Step-2: Enter http://IPAddress:8000/ in a browser to see the application running.
