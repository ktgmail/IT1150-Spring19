# Visual Studio Code and GitHub Setup


### Download Visual Studio Code
Download Visual Studio Code from https://code.visualstudio.com/download

### Create a GitHub account
[GitHub](https://github.com/)

### Fork a Copy of our class GitHub repo
1. Log into your GitHub account use the search box to find our class respoitory:IT1150-Spring19
2. Select the repository and click the "Fork" in the upper right corner of the GitHub window
3. [Understanding Forking](https://help.github.com/articles/fork-a-repo/)

### Install GitHub
Install the GitHub command line tool. https://git-scm.com/

### Clone your GitHub repository
"Cloning" a repository means you are making a local copy on your computer.  If using a lab computer delete the file once commits are made.

First change to the directory where you want to store a local copy of your source code files: Open a command prompt. Press the Windows key and search for "cmd". Press enter to open the command prompt. From here we'll enter command prompt calls to clone your repository.

Note: cloning will create a copy of your remote repository on your computer. It will create a folder with the same name as your repository.

First copy your repository URL. For example, our class repository has the URL: https://github.com/ktamerl4/IT1150-Spring19. I'll use this in place of your repository link for the following examples.

```
git clone https://github.com/ktamerl4/IT1150-Spring19
```

### Configure user name and email address for local git cache - this portion is for your personal computer only
Change directories into the folder that was just created for your cloned repository. Example:
```
cd repository_folder_name
```
Now, use the following commands to configure cached settings for your repository. This is the email and name that will be logged with any commits to the repository.
```
git config --global user.name "John Doe"
git config --global user.email "johndoe@example.com"
```
You can double-check to make sure the settings were applied using the following command:
```
git config --list
```

### Download / Pull Any Changes that were Made to the Repository Outside of your Local Copy
If you're opening a new command prompt window in the future, you'll always have to change the current working directory to the folder that you cloned your repository to. 
```
cd path_to_repository
```

To download/pull changes from the remote repository to your local repository:
```
git pull
```

### Commit and Push Files to the Repository
Again, make sure you're in the folder for your local repository. Type the following command to add any new files that you created since the last commit:
```
git add .
```
Now, commit all of the files that have changed or were added.
```
git commit -m "Commit Message"
```
Now, push (upload) all files that were changed to your remote repository.
```
git push
```
