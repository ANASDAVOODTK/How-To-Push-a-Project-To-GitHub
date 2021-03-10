# How-To-Push-a-Project-To-GitHub

The existing commands can be simply run via the CLI terminal of VS-CODE. It is understood that Git is installed in the system, configured with desired username and email Id. <link>https://code.visualstudio.com/docs/editor/github</link>

### 1) Navigate to the local project directory and create a local git repository:

        git init
        
        git add .   //for adding all your code for commit. if already done just ignore it
        
        
        
### 2) Once that is successful, click on the 'Source Control' icon on the left navbar in VS-Code.One should be able to see files ready to be commit-ed. Press on 'Commit'                 button,  provide comments, stage the changes and commit the files. Alternatively you can run from CLI

         git commit -m "Your comment"
 
### 3) Now you need to visit your GitHub account and create a new Repository. Exclude creating 'README.md', '.gitIgnore' files. Also do not add any License to the repo. Sometimes        these settings cause issue while pushing in.

### 4) Copy the link to this newly created GitHub Repository.

### 5) Come back to the terminal in VS-CODE and type these commands in succession:

       git remote add origin <Link to GitHub Repo>     //maps the remote repo link to local git repo

       git remote -v                                  //this is to verify the link to the remote repo 

       git push -u origin master                      // pushes the commit-ed changes into the remote repo


  Note: If it is the first time the local git account is trying to connect to GitHub, you may be required to enter credentials to GitHub in a separate window.

### 6) You can see the success message in the Terminal. You can also verify by refreshing the GitHub repo online.

Hope this helps
