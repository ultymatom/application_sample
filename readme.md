# Introduction
This project is a basic application to show how we advice you to create your repository.
It is a simple web server that you can build and run with any container engine.

#Gitflow
This paragraph is only to explain the gitflow, in a regular project you do not need to add it.

*develop*: It is the development branch, when you want to add a new feature, you create a new branch from it. Once your developments are done, you can merge your branch into develop where a chain of tests should be played on it to validate the developments. +

*master*: This is the branch containing all finished and validated development. The only commits received by this branch should only be merge received from *develop* when your chain of tests have been played successfully on it. +
All release should be created from this branch

*feature/<team_or_developper_name>/<name_of_feature>*: We here choose a template for the name of features branch, feel free to use another one you prefer. The features branches are created from *develop*, they are used by a developer (or a team of developers) when working on a new feature (the process when fixing a bug can be the same also). Once the feature is working, the developer can merge his modification in *develop* where it can be validated.

*release_<version>*: We here choose a template for the name of releases branch, feel free to use another one you prefer. These branches should be created from *master*, they are branches that are supposed to be deployed on production.

NOTE: With this gitflow your *master* need to be protected, in this repository for example we used these options +
*TBD*

# Getting Started
TODO: Guide users through getting your code up and running on their own system. In this section you can talk about:
1.	Build the application
  You can build your application with container engine as docker or podman, here we will write example with docker, but if you replace docker with podman it will work exactly the same. +
  `docker build -t <tag> .` (to be executed inside the application repository)
2.	Run the application
  `podman run --name <container name> <image tag> -d -p 8080:<local_port>`
3.	Accesing the web server
  Open any browser and connect to <ip_address_of_host>:<local_port>


# Build and Test

1. Build (same as 1. of getting started)
  You can build your application with container engine as docker or podman, here we will write example with docker, but if you replace docker with podman it will work exactly the same. +
  `docker build -t <tag> .` (to be executed inside the application repository)

2. Tests
For this sample we did not make a chain of tools for testing, but in this part you should explain what tools you use to test your development.

# Contribute
TODO: Explain how other users and developers can contribute to make your code better.

If you want to learn more about creating good readme files then refer the following [guidelines](https://docs.microsoft.com/en-us/azure/devops/repos/git/create-a-readme?view=azure-devops). You can also seek inspiration from the below readme files:
- [ASP.NET Core](https://github.com/aspnet/Home)
- [Visual Studio Code](https://github.com/Microsoft/vscode)
- [Chakra Core](https://github.com/Microsoft/ChakraCore)
