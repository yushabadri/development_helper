<p align="center"><a href="https://laravel.com" target="_blank"><img src="assets/Git-Logo-2Color.png" width="250" alt="Laravel Logo"></a></p>

<p align="center"> Command Hepler For GIT</p>




This guide will help you connect a project from the base to the gate and work with it using Git.

### Create a New Empty Repository

The first step is to create a new empty repository on GitHub.

### Connecting Local Project to an Existing Git Repo

To connect your local project to Git, follow these steps:

1. Open your terminal and navigate to the root directory of your project.
2. Run the following command to initialize Git: 

    ```
    git init
    ```

3. Run the following command to add the remote origin URL:

    ```
    git remote add origin https://github.com/directory/name.git
    ```

   Note: Replace `https://github.com/directory/name.git` with the actual remote origin URL.

4. Run the following command to rename the default branch from `master` to `main`: 

    Renaming the default branch from master to main is a good practice, considering the more inclusive and neutral term. This step is optional but recommended.

    ```
    git branch -M main
    ```

5. Run the following command to stage all changes:
    
    <span style="color:red">Note</span> : stages all changes in your project for the commit. This is correct, but be mindful of what you're adding; you don't want to include unnecessary or sensitive files.

    ```
    git add .
    ```

6. Run the following command to set your Git user email:

    ```
    git config --global user.email "email@address"
    ```

   <span style="color:red">Note</span> : Replace `"email@address"` with your actual email address.

7. Run the following command to set your Git user name:

    ```
    git config --global user.name "Your Name"
    ```

   <span style="color:red">Note</span> : Replace `"Your Name"` with your actual name.


8. Run the following command for pulling Changes with Unrelated Histories:

    <span style="color:red">Note</span> : This step is important when you're pulling from a remote repository that already has content. It helps to merge the unrelated histories in case you've started your local repository with different commits.

    ```
   git pull origin main --allow-unrelated-histories
    ```

9. Run the following command to make the initial commit:

    ```
    git commit -m "initial commit"
    ```
     The "initial commit" message is common for the first commit of a project

10. Run the following command to push the changes to the remote repository:

    ```
    git push -u origin main
    ``` 
    
  

   Note: If you encounter an error about authentication, make sure you have the correct permissions to push to the repository.

That's it! Your local project is now connected to Git and pushed to the remote repository.
