# Automating Build, Package and Deployment of Power Platform Solutions with GitHub Actions

## Credit
This project was adapted from the [MicrosoftDocs/power-platform](https://github.com/MicrosoftDocs/power-platform/tree/main/power-platform/alm/tutorials) repository. All credit goes to that team for their hard work and dedication to the community.

## Getting Started
This project uses GitHub Actions, an Azure AD service principal, and Power Platform Solutions to automate building, packaging, and deploying apps. The solution is split into three Dataverse environments for development, build, and production, each with its own application user.

To use this project, please follow the steps outlined in the following links:

| Link                                          | Description                                                                                                                                                                                                 |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [github-actions-start.md](https://github.com/MicrosoftDocs/power-platform/blob/main/power-platform/alm/tutorials/github-actions-start.md)   | Steps to setup GitHub Actions and Azure AD service principal.                                                                                    |
| [github-actions-build.md](https://github.com/MicrosoftDocs/power-platform/blob/main/power-platform/alm/tutorials/github-actions-build.md)   | Steps to automate building the solution using GitHub Actions.                                                                                                              |
| [github-actions-deploy.md](https://github.com/MicrosoftDocs/power-platform/blob/main/power-platform/alm/tutorials/github-actions-deploy.md) | Steps required to automate deploying the solution to the three Dataverse environments.                                                                                              |

> **Note**
> The application user must be added to all three environments.

````
                                    +----------------------------------+
                                    |      github-actions-deploy.md    |
                                    +----------------------------------+
                                                ^
                                                |                        
                                                |               
                  +-----------------------------------+     
                  |      github-actions-build.md      |     
                  +-----------------------------------+
                              ^    
                              |                     
                              |               
+-----------------------------------+     
|      github-actions-start.md      |
+-----------------------------------+
````

## Additional Resources

- [Git Tagging](https://git-scm.com/book/en/v2/Git-Basics-Tagging): How to use Git tags to manage releases.

