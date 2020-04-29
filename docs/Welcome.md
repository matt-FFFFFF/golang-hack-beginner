# Welcome!

First and foremost, welcome to the Golang hack! We are excited for you to join us, whether you're a n00b or an experience Golang developer.  In this hack we are offering a few different tracks for you to choose from that will help you learn Golang no matter your level of expertise (or none at all).  

This hack was devised from an idea from April Edwards and Matt White.  We were both learning Golang and wanted to find others that wanted to learn.  We wrote this hack to bring us GOphers together and collate learning materials and resources for everyone.

This hack was designed to run over 2 days.  The aim is to provide learning materials, a learning path and a sense of community with your team (and the wider community).  Your teams have been divided up by skill set.


# Getting Started

Before the start of the hack, it is highly recommended to review the pre-req's below.  Please make sure you have your machine setup before the hack begins.

We ask that everyone participating in the hack to have completed the [Golang tour:](https://tour.golang.org/welcome/1)

We have outlined some tools/software that you will need to complete the challenges.


## Pre-requisites

You will need to setup your machine for the hack, so let's get your environment set up

### GitHub

You will need a GitHub account for this, please ensure you have one. One member of your team will fork the repo and invite the others as collaborators.

### Exercism

The learning modules that we have set up will use Exercism, it is recommended for the Level zero and Level 100 teams to complete these (not compulsory, but highly recommended).  You can sign up for an Exercism account before the hack starts:[Exercism](https://exercism.io/)

## Setting up your machine

You will need to setup your machine ready to code Go. The following directions apply to Windows users, we assume that you're running Windows 10. We would suggest following the steps in order, as listed, to avoid spending hours troubleshooting any installation related issues. 

### VS Code
1. Install [Visual Studio Code](https://code.visualstudio.com/) - Accept the defaults when installing.

2. Configure Visual Studio Code with extensions

   Open VS Code, then press ```CTRL+SHIFT+X``` to view the extensions.
   Search for and install the following extensions.

   First press ```CTRL+p``` to enter *quick open*.
   Then type:

      ```ext install ms-vscode.go```

3. Repeat this process and install:

   * ```ms-vscode-remote.vscode-remote-extensionpack```
   * ```ms-azuretools.vscode-docker```
   * ```ms-vsliveshare.vsliveshare```


### Git for Windows
 1. Go uses open source repositories, you will need to install [Git for Windows](https://git-scm.com/download/win)

 2. Accept the defaults for the installation. **NOTE:** Ensure the default editor is Visual Studio Code

### Go for Windows
1. Navigate to [Go for Windows](https://golang.org/dl/)

2. Download and install the latest 64-bit Go bit for Microsoft Windows OS

3. Follow the instructions on the installation

4. After the install completes, run 'Command Prompt' and type: 'go version'   You should see a go version of 1.x installed

5. Confirm your Go workspace.  You will need to create the Go workspace where you will run your Go projects from.  The Go workspace will contain two directories at its root:

   *src*: The directory that contains Go source files. A source file is a file that you write using the Go programming language. Source files are used by the Go compiler to create an executable binary file.

   *bin*: The directory that contains executables built and installed by the Go tools. Executables are binary files that run on your system and execute tasks. These are typically the programs compiled by your source code or another downloaded Go source code.

   a) Confirm your Go binaries by going to Control Panel>System and Security>System>Advanced system settings.  On the left had pane click the 'Advanced' tab  
   
   b) Click on 'Environment Variables' on the bottom right hand side
   
   c) Ensure 'Path' under System Variables has the "C:\Go\bin" variable in it

   d) After setting your environment variable, you will need to create your Go workspace.  This will be a separate folder to where your Go install files are saved. Your Go install files were saved under 'C:\Go', your new workspace you should be in 'C:\Users\%USERNAME%\Go'  You can browse to that folder and see 3 other folders: bin, code, src (If you do not see those folders, you will need to create them).  Your directory structure should look like this:

   .
   +--%Username%
   |  +--go
   |  ++--bin
   |  ++--src

     └── %Username%
         └── go
            ├── bin
            └── src
            

6. Create the GOPATH Environment Variable and reference your newly created Go workspace.  Navigate back to your Control Panel>System>Environment Variables>System Variables  - Select 'New'

      Variable name: 'GOPATH'
      Variable Value: 'C:\Users\%USERNAME%\Go'

   a) Save the above changes then open Command Prompt and enter: 'echo %GOPATH%'  - Ensure that the path has been set correctly, else go back through and check your settings.

### Postman

Download [Postman](https://www.postman.com/downloads/) - Follow the defaults and install

### Docker for Windows

Download and install [Docker for Windows](https://download.docker.com/win/stable/Docker%20Desktop%20Installer.exe) - Please follow the defaults for installation

### Windows Terminal 

While not required, it is recommended [Windows Terminal](ms-windows-store://pdp?productId=9N0DX20HK701) 

### Optional Configurations

VS Code can run Dev Containers, read about it here **LINK**

Add details***


# Getting Started in Your Team

We asked each person to register and provide their approximate skill set. Thus, we have created a sort of 'create your own adventure' style of learning.  From  your teams you will be with like leveled individuals so that hopefully everyone is at a similar starting point in their learning journey.  It is suggested that you work together as a team, whether it be as a whole team, pair programming or asynchronously.  It is entirely up to your team.  It is important to setup some form of repo for the team and a Microsoft Teams site to communicate (unless one has already been provided).

We have defined the skill levels based on the tasks that we have setup:

 *Level Zero*: n00b, never coded with Golang but are super eager to learn
 *Level 100*: have dabbled in Golang, maybe 'Hello World' or something simple
 *Level 200*: Some coding in Golang, looking for your next learning challenge or a real-life example
 *Level 300 - 400*: Very experienced, or expert level. Still hoping to learn a bit more.

Once in your team, discuss which path of the hack you would like to explore as a group.  We have outlined some suggestions to help you understand what each path entails:

Suggested path per skill level:

 **Level Zero - 100:** Day 1, it is worth reviewing the Go tour with your team and make sure everyone is comfortable with the concepts. This is a great time to review with the team the topics learned and make sure there aren't any questions.  

   *Next phase:* once your team has completed the review of the Go Tour, we highly recommend going through the next level of exercises, learning loops and arrays, we called this 'Ground Zero'.  We have setup 2 tasks using Exercism, it is highly recommended you start with those learning modules before moving onto the core of the hack, the Book API Challenge. The link to get started on 'Ground Zero' will be found at the bottom of this document.

   Suggested Path:  Golang tour --> Ground Zero --> Book API Challenge

**Level 200:** Your group can choose to warm up your skills by completing the learning tutorials on loops and arrays before proceeding to the Book API (Challenge 1).  The learning tutorials are hosted in Exercism. We suggest that your group decides on where they would like to start  Else, you can proceed straight to the Book API Challenge

**Level 300 - 400:** There is an assumption that you're very familiar with the concepts in the Go tour.  You will go straight to your Auzre Auto Tag Challenge written by Gabriel Nepomuceno. You may also choose to complete the Book API path as a warmup before proceeding to the main challenge, it is comprised of 4 challenges

# Let's Get Hacking

We have outlined the setup and now it's time to get hacking.

This is where your team will need to decide which challenge to start with we have created a 'choose your own adventure' model.  We have suggested where we think each team would benefit from most. Pick your path:

      First Header       |    Second Header
  -----------------------|-------------------------
  GoLang Tour (review)| https://tour.golang.org/
  Content Cell        | Content Cell





You now have a choice. You can start with a couple of warm up exercises in [ground zero](GroundZero.md)...

Or, you can get start the hack with [hello world](helloworld.md)