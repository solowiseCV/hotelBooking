# hotelBooking

## Explain version control.

Version control, also known as source control, is the practice of tracking and managing changes to software code. Version control systems are software tools that help software teams manage changes to source code over time.
Here are some concepts of version control

 - Repository:
    A repository (repo) is a central storage location where all the files, history, and metadata related to a project are stored.
    Repositories can be either centralized (single repository on a server) or distributed 

 - Commits:
    A commit represents a snapshot of the project at a specific point in time.
     It includes changes made to files, a commit message describing the changes, and metadata like the author and timestamp. 

 - Branching:
   Branching allows for the creation of separate lines of development within a repository.
   Each branch is an independent series of commits, and users can work on different features or fixes without affecting the main codebase until they are ready to merge their changes.  

 - Merging:
     Merging is the process of combining changes from one branch into another.
     It is typically used to integrate new features or bug fixes back into the main branch.

 - Remote Repository:  
     In distributed version control systems, there is often a remote repository that serves as a central point for collaboration.
      Users can push their changes to the remote repository and pull changes from it to stay synchronized with the latest developments.  

 - History: 
     Version control systems maintain a complete history of changes made to a project, allowing users to review and revert to previous states if needed.
      This historical record helps in understanding who made a particular change, when it was made, and why.

  ## Explain difference between git and github
     
  - Git:  
     Definition:Git is a distributed version control system designed to track changes in source code during software development. It is open-source and was created by Linus Torvalds.
     - Functionality:
        Git provides the core version control functionality, allowing users to create and manage repositories, make commits, create branches, and merge changes.
     - Local:
         Git operates locally on a user's machine. Developers can work on their projects without needing an internet connection or a central server. 
     - Command Line:
         Git is primarily used through the command line, although there are graphical user interfaces available for those who prefer a visual interface.while github is   
        
   - GitHub:
      Definition:GitHub is a web-based platform that provides hosting for software development projects that use Git for version control.
     - Hosting and collaboration:
        GitHub is a web-based platform that provides hosting for software development projects that use Git for version control.
     - Integration: 
         GitHub integrates with various third-party tools, and it has become a standard platform for open-source development, as well as for many private repositories.
     - Web Interface:
          GitHub offers a web-based interface that simplifies collaboration. Users can manage repositories, create issues, perform code reviews, and more through the web interface.
     - Social Features:
         GitHub includes social features such as pull requests, forks, stars, and followers, making it a social platform for collaboration and community involvement.

## List 3 other github alternatives
   
   *Three other github alternatives are*
    - GitLab
    - Bitbucket
    - SourceForge

## Explain the difference between git fetch and git pull
   
   git fetch and git pull are both Git commands that involve fetching changes from a remote repository, but they serve slightly different purposes.
    - git fetch:
        Fetching is the operation where you retrieve the latest changes from a remote repository but do not automatically merge them into your working branch.
        It updates your local repository with any new branches or commits from the remote repository.
        The command does not modify your working directory or the branch you are currently on. while git pull
    - git pull :
         Pulling is a combination of fetching and merging. It fetches the changes from the remote repository and automatically merges them into your current working branch.
         Essentially, git pull is equivalent to running git fetch followed by git merge.
         This command is useful when you want to update your working branch with the latest changes from the remote repository and immediately incorporate those changes into your local files. 

   ## Explain in simple terms git rebase and the command for it

     -Rebase:
       definition:Git rebase is a command used to integrate changes from one branch into another by moving or combining a sequence of commits. It essentially rewrites the commit history, producing a cleaner and more linear project history. The primary use case for rebase is to maintain a clean, logically organized commit history, especially when working on feature branches.
       Here's a basic overview of how rebase works:
        - Starting Point:
           Assume you have a feature branch with some commits, and there have been additional commits on the main branch (or any other branch).
        - Initial rebase:
            You switch to your feature branch and run the rebase command:
               ```git checkout feature-branch
                     git rebase main``` 

         - Resolve Conflicts:
            If there are conflicts between your changes and the changes in the main branch, Git will pause the rebase process and ask you to resolve the conflicts.
         - Continue Rebase:
            -  After resolving conflicts, you continue the      rebase process with the Command line:
               ```git rebase --continue```
         - Finish Rebase :
             - Once the rebase is complete without conflicts, your feature branch now includes all the changes from the main branch, and the commit history appears more linear.
             
        It's important to note that rebase should be used with caution, especially on shared branches. Rewriting history can make collaboration more challenging, as it alters commit IDs. Therefore, it's generally recommended to use rebase on local feature branches before sharing them with others.

   ## Explain in simple terms git cherry-pick and the command for it 
              
     
      - In simple terms, ```git cherry-pick``` is a command that lets you copy specific commits from one   branch and apply them onto another branch. It allows you to pick and choose individual changes and bring them into a different branch without merging the entire branch.
       - Here's a basic explanation and the command for ```git cherry-pick``` :
         - senario:
            You have different branches in your Git repository, and you want to copy a specific commit from one branch to another.