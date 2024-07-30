<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GIT Notes</title>
</head>
<body>
    <h1>Git Knowledge - the example below is when you Clone a project from github repo.</h1>
    <ol type="1">
        <li>Version Control is <b>Git.</b></li>
        <li>To create a new repo, press new repo on the github dashboard. Below are some key points to note: <br>
        <ol type="A">
            <li>Name your repo.</li>
            <li>Choose between public and private</li>
            <li>Description is optional</li>
            <li>Initialize this repo: entails that you can also create a README file, which can be altered using html tags in the dashboard. <i>When making changes on the readme file, you can click on <b>Commit Changes on the right side window and describe your changes.</b></i> See below <br>
            <img src="/images/04.PNG" alt=""></li>
            
</ol></li>
        <li><b>Setting up Git</b>:
        <ol type="A">
            <li>VS Code install</li>
            <li>Windows git bash from git.com</li>
            <li>git --version : entails the installation of git.</li>
        </ol></li>
        <li>Free and Open Source. Fast and scalable.</li>
        <li>Connect with your web github using the following commands:
            <ol type="a">
                <li><b>git config --global user.name "sohaib"</b></li>
                <li><b>git config --global user.email "sohaib.sharih@gmail.com"</b></li>
                <li><b>git config --list</b> indicates all your settings.</li>
                <li>The purpose of <b>git configuration</b> is to tell <b>git</b> the details of the user + user's account you will be applying changes to or working with.</li>
                <li><b>Note:</b>This allows you to setup your github account and integrate with your local vscode so you don't have to connect each time you perform git init command. All that your <b>push</b> and <b>pull</b> requests will be done through the <b>global settings.</b></li>
            </ol>
            
</li>
        <li><b>Git clone</b> to copy the github repo files to your <b>local</b> machine. <b>git clone 'url of repo'</b> <i>By default, the name of the repository is <b>origin.</b></i><b>Git Clone command</b> also entails that once you clone a repo from the link, it also downloads the <b>.git config folder + files</b> into your <b>local machine.</b> </li>
        <li><b>Git status</b> provides the status of the code. See below <br>
        <img src="/images/01.PNG" alt=""> <i>if there are any changes made, then you will be prompted to add them to staging, then commit, then to push your code if you wish to do so.</i></li>
        <li><b>ls</b> command provides a list of files in your current directory.</li>
        <li><b>ls -a</b> provides a list of all the files, including the hidden files.</li>
        <li><b>use git bash CLI</b></li>
        <li><b>Git Commit</b>, this is done after adding changes to the stage. Command => git commit -m "some mssage"</li>
        <li><b>Untracked files:</b> If we create a new file, it will be marked U, which is untracked in git, therefore we need to <b>add</b> it to staging. See below: <br>
        
<img src="/images/02.PNG" alt=""></li>
        <img src="/images/03.PNG" alt="">
        <li><b>git add .</b> denotes that all files in the folder need to be <b>staged.</b> Whereas <b>git add 'name of file with extension'</b> is used to <b>stage</b> a particular file.</li>
        <li>There are 4 different types of <b>git statuses:</b>
        <ol type="a">
            <li><b>Untracked</b>: Are those files that are not tracked, but were created. You need to <b>add</b> them to the git config by running the <b>git add</b> command.</li>
            <li><b>Modified</b>: If we make any changes to <b>tracked files</b>, then its marked <b>Modified.</b> </li>
            <li><b>Staged</b>: means that files were staged, ready to be <b>committed</b> and <b>pushed.</b> A file is ready to be committed.</li>
            <li><b>Unmodified:</b> means that the file is being tracked, but no changes were made to it after adding all other files to stage.</li>
            <li><b>Note:</b>We use <b>Add & Commit</b> commands to add the files to the <b>staging area.</b>Whereas as, <b>git commit -m</b> is what makes a record of the change you recently made.</li>
        </ol></li>
        <li><b>git push origin main</b>: <b>origin</b> denotes the name/connection name of the repository, and <b>main</b> denotes the name of the <b>branch.</b> <i>The default name of <b>connection</b> when <b>cloning</b> a repo to your local system is <b>origin</b>, therefore you need to use the <b>git push origin main</b> command.</i></li>
        <li><b>git remote -v</b> provides the current version of your git connection.</li>
        <li><b>git init command</b>: initialises the directory in which you are currently working on your local machine.</li>
        <li><b>How to create a new branch?</b>
        <ol type="A">
            <li><b>git branch <i>'mention the name here'</i> </b></li>
            <li><b>git checkout 'nameOfBranch'</b>: will allow you to switch the branch on your local repo.</li>
            <li><b>git push origin 'nameOfnewBranch'</b>: It will allow you to push the new changes in your <b>git hub repo.</b> And the <b>new branch</b> will be added to your github repo <b>along with the recent changes you applied.</b></li>
            
</ol></li>
        <li>The general sequence:
            <ol type="A">
                <li><b>git clone</b> 'repo link/url' to import the files from the github repo.</li>
                <li><b>git add .</b> => adds all files to the staging area.</li>
                <li><b>git commit -m 'message'</b> => adds all changes to the record.</li>
                <li><b>git push origin main</b> => pushes the changed and tracked files to the repo.</li>
                <li>Before you push, if you want, you can either <b>rename the current branch (git branch -M 'name')</b> or add a new breanch by using <b>git branch 'name of branch'</b> then you do that before pushing.</li>
            </ol>
        </li>
    </ol>

<h1>How do we prepare a project in our Local Drive?</h1>
    <ol type="1">
        <li><b>git init</b></li>
        <li><b>Create a file</b> and use <b>git add .</b></li>
        <li><b>git commit -m "description of change"</b></li>
        <li><b>Create a new repo on git hub</b>: without initializing README.me. <i>If you initialize it, then the default branch name becomes <b>main.</b></i> <br>
        <img src="/images/05.PNG" alt=""></li>
        <li><b>git remote add origin 'repo link'</b>: <i>this helps to build a connection with the github repo.</i><i>This command also helps to create <b>the name of the repo connection/remote connection</b></i></li>
        <li><b>git push origin main</b> OR <b>git push newOrigin main</b></li>
        <li><b>git push origin 'nameOfBranch'</b>: entails that you can <b>push</b> a <b>new branch</b> that you have created in your <b>local directory.</b> It can be a totally new branch being added to the <b>github repo.</b></li>
        <li>To change the name of the <b>current branch</b>, use <b>git branch -M 'name of branch'</b>: <i>This command only helps to replace the current name of the branch.</i></li>
        <li>To push the files to the repo, simply use <b>git push -u origin main</b>. -u is used to make sure that if you want to set <b>upstream</b>, it allows you to then simply use <b>git push</b> rather than always writing the full command <b>git push origin main</b></li>
        <li></li>
        <li><b>Note:</b> default branch on github now is called <b>main</b>, before it used to be <b>master.</b> This is when you create a new repo along with <b>readMe.me file intialization.</b></li>
    </ol>


<h1>How to create a new Remote Connection/name?</h1>
    <ol type="1">
        <li>git remote -v : provides the current remote connections to your <b>local directory.</b></li>
        <li>git remote add 'nameOfConnection' 'linkOfGitHubRepo': This will allow you to create a <b>new name of connection</b> and also the link is required to connect your <b>local directory/repo</b> with the <b>github repo.</b></li>
        <li><b>origin</b> is a <b>default</b> connection name.</li>
        <li>Note: You should call it MAIN, as its a name used most commonly. The first time you create a new name for connection, <b>automatically becomes</b> part of the <b>default connection name.</b></li>
    </ol>

<h1>Git Branches</h1>
    <ol type="1">
        <li>We can <b>clone</b> or create a <b>new repo by initializing it in your local directory.</b> And work on a new branch, then commit it and push it as a new branch, or switch to the existing/similar branch as the git hub repo branch and then <b>push it.</b></li>
        <li>Git branch commands
            <ol type="A">
                <li><b>git branch</b> provides the list of branches and indicates which branch you are at.</li>
                <li><b>git branch -M main</b> <i>to <b>rename</b> an existing branch you are on.</i></li>
                <li><b>git checkout 'branch name'</b> <i>to navigate/switch to another branch.</i></li>
                <li><b>git checkout -b 'new branch name'</b>: <i>to <b>replace</b> the name of an existing branch with a <b>new branch name</b>, and also <b>switch simaltaneously.</b> Its a quick way to replace + switch</i> <b>Note:</b> this allows to copy all your last commits to the newly created branch.</li>
                <li><b>git branch -d 'branch name'</b>: This deletes the branch. <i>You have to switch to another branch in order to delete the branch you are currently on. In other words you cannot delete the branch you are currently on.</i></li>
                <li><b>Note:</b> You cannot create a new branch until you have made your first commit.</li>
            </ol>
        
        </li>
<li><b>Merging Code</b> 
        <ol type="A">
            <li><b>Method 1</b>
            <ol type="i">
                <li><b>git diff 'branch name'</b>: <i>to compare 2 branches, their commits and files.</i> <br>
                <img src="/images/06.PNG" alt=""><b>git branch -> newFour</b>
            <img src="/images/07.PNG" alt=""><b>git branch -> newOne</b> <br>
        <img src="/images/08.PNG" alt=""><br>When you run the command to compare git diff 'mentionTheNameOf the branch that you want to compare your CURRENT branch with.'</li>
                <li><b>git merge 'branch name':</b> <i>to merge 2 branches.</i></li>
            </ol></li>
            <li><b>Method 2: CREATE PR (Pull Request)</b>
            <ol type="i">
                <li>Definition of <b>PR</b>: It allows others to know about the <b>changes</b> you've pushed to a branch in a repository on GitHub.</li>
                <li><img src="/images/10.PNG" alt=""></li>
                <li><img src="/images/11.PNG" alt=""></li>
                <li>Scroll down and click on  Merge Request button at the bottom</li>
                <li><img src="/images/12.PNG" alt=""></li>
                <li><img src="/images/13.PNG" alt=""></li>
                <li><img src="/images/14.PNG" alt=""></li>
                <li><img src="/images/15.PNG" alt="">Now you can see the <b>New Commit during Merging process.</b></li>
                <li>To createa  new Pull Request, you can always go to pull request section and choose between branches to compare, if only there are differences in files, then you can describe and request for a <b>change.</b></li>
                <li><b>git pull origin main</b> request can be used whenever you want to <i>get the changes of github repo to <b>local repo/directory.</b></i>It is used to <b>fetch</b> and <b>download</b> content from a remote repo and immediately update the local repo to match that content.</li>
                
</ol></li>
</ol></li>
</ol>
<h1>Merge Conflicts</h1>
    <ol type="1">
        <li>When you make a change within the same html tag in both branches but with different text or feature like adding a <b>button</b>, then the below conflict occurs: <br>
        <img src="/images/16.PNG" alt=""></li>
        <li>When git is unable to resolve the differences within the <b>same places</b>, then it gives a <b>conflict as shown above.</b></li>
        <li>We can delete the conflicts manually as shown below and decide what to keep: <br>
        <img src="/images/17.PNG" alt=""></li>
        <li> Save the changes, then do the following: <br>
        <img src="/images/18.PNG" alt=""></li>
        <li> You can then follow the same process of Git Merging, you can use the command <b>git merge 'nname of branch that needs to be merged with the current one you are on.'</b></li>
    </ol>

<h1>Undoing Changes.</h1>
    <ol type="1">
        <li><img src="/images/19.PNG" alt=""></li>
        <li></li>
    </ol>

<h1>How to change the default branch name?</h1>
    <ol type="1">
        <li><b>Case 1: </b>You can go to git hub repo, and click <b>branches</b>, then from the 3 dots, select 'Rename branch' under the <b>section</b> of <b>default.</b> <br>
        <img src="/images/09.PNG" alt=""></li>
        <li>Once you've added a new change in a file, and also used the <b>git add .</b> command to stage it, but haven't committed yet.</li>
        <li>Then you can use the command git reset 'name of file with extension'</li>
        <li><b>Case 2:</b>Committed changes for a single/1 commit.
        <ol type="A">
            <li><img src="/images/20.PNG" alt=""></li>
            <li><b>git reset HEAD~1</b>: allows you to <b>uncommit</b> and move 1 step backwards and then makes your file indicate <b>M</b> <br>
            <img src="/images/21.PNG" alt=""></li>
            <li>If you want to move <b>backwards</b> you can check the <b>hash</b> from <b>git log</b> to move or jump to that particular change. You can use the has in <b>git reset 'enter hashkey'</b> shown below: <br><img src="/images/22.PNG" alt=""></li>
            <li>To see how to use the git reset hashkey command: <br>
            <img src="/images/23.PNG" alt=""></li>
            <li>When using the hashkey, or when resetting, then a <b>green line appears to indicate the reset and changed lines</b> <br>
            <img src="/images/24.PNG" alt=""></li>
            <li>In order to remove the changes along with the command we use <b>git reset hashkey</b>, we can use the command <b>git reset --hard090798987453499</b></li>
            
        </ol></li>
    </ol>

<h1>FORK</h1>
    <ol type="1">
        <li>Fork: This entails that when you want to have a <b>rough copy</b> of the code of someone else's git hub, that will include the code + visibility settings with the original upstream repository. </li>
        <li>This can be done when you want to <b>Contribute.</b></li>
        <li>To fork, you should do the following: <br>
        <img src="/images/25.PNG" alt=""></li>
        <li><img src="/images/26.PNG" alt=""></li>
        <li>You can then commit changes within your own repo of main/master branch of your github repo.</li>
        <li>You can then go to <b>PULL REQUEST</b> <br>
        <img src="/images/27.PNG" alt=""></li>
        
</ol>

<h1>Git Ignore: How to ignore files and folders</h1>
    <ol type="1">
        <li><b>git ignore</b> is essentially used to indicate files and folders that need not be pushed on to github, since any other developer who wants to use the files to run them locally, can simply use <b>cli commands</b> for example, when using libraries and modules of <b>npm.</b>, they can simply run the installation commandst to install all the required files that are mentioned in <b>package.json</b>file.</li>
        <li><b>Configuration files</b>Secondly, another reason to ignore files and folders is to keep the code lightweight when uploading them to github repo, as other 3rd party modules and libraries may be heavy files and may take up unnecessary storage space.</li>
        <li><b>Sensitive files</b>: such as .env files or other files containing passwords, can be ignored using git ignore.</li>
        <li><b>Steps:</b>
        <ol type="A">
            <li>use <b>touch .gitignore</b> cmd to create the file.</li>
            <li><b>Ignoring a file:</b> If you want to ignore a specific file, you will have to provide the <b>full path</b> of the file location from the <b>root folder</b>, along with its extension. Example /test/text.txt OR test/text.txt <i>can write both ways.</i></li>
            <li>To ignore a specific file (e.g., index.html in the root directory): <br>
            <b>index.html</b></li>
            <li>Example for files in a specific directory: <br>
                If the file is in a subdirectory, include the path relative to the repository root: <br>
                <b>subdirectory/example.html</b></li>
            <li>To ignore all HTML files in a specific directory, use: <br>
            <b>subdirectory/*.html</b>            </li>
            <li>To ignore all HTML files throughout the repository, add: <br>
                <b>*.html</b>            </li>
            <li><b>Remove the File from the Staging Area</b>. <i>If the file is already tracked by Git (i.e., has been committed before), you'll need to untrack it before it can be ignored. Use the following command:</i> <br>
            <b>git rm --cached 'file-path'</b> <br>
            For example, if you're ignoring index.html: <br>
            <b>git rm --cached index.html</b> <br>
            <b>Note:</b> This command will remove the file from the Git index but keep it in your working directory.
                </li>
            <li><b>Commit the Changes</b>. <i>Commit the updated <b>.gitignore</b> and any changes from the <b>untracked file</b>:</i> <br>
                <b>git add .gitignore <br>
                    git commit -m "Add index.html to .gitignore"</b>
                </li>
            
</ol></li>
    </ol>

<h1>Situation: If you have pushed all the wrong files and folders and want to push a new set of files and folders, what do you do?</h1>
    <ol type="1">
        <li>A similar situaion occured with me because i didn't initialize the git on my working directory.</li>
        <li>But i was still able to push the contents to the remote repository. I discovered, this happened because the <b>name of connection</b> was similar to a <b>parent folder</b> that was already <b>initialized</b> before. So while <b>pushing</b>, it took all the <b>staged files and folders</b> that were <b>committed</b> in that specific <b>branch name</b> and <b>connection name</b>. </li>
        <li>Steps to fix the above mentioned situation:
            <ol type="a">
                <li><b>Clone</b> the git repo to a <b>new folder</b></li>
                <li>use the <b>git rm 'nameOfFile'</b> command to delete each file, and <b>git rm -r 'directoryName/foldername'</b> OR simply delete all the files and folders manually.</li>
                <li>run the <b>git add .</b> command to stage all the new changes. If it doesn't work, create a single file and do this.</li>
                <li>run the <b>git push 'nameOfConnection' 'nameOfBranch'</b></li>
                <li>It may not work due to <b>conflict</b>, therefore you can use the <b>--force</b> flag. example <b>git push newOrigin main --force</b></li>
                <li><b>Note:</b> the force flag is however not a good practice if you are working in a <b>collaborative team</b> environment.</li>
            </ol>
        </li>
        <li><b>Method 2</b>
        <ol type="a">
            <li><b>Clone</b> the remote repository inside a <b>new folder</b></li>
            <li>delete the <b>gitignore file</b>, then create a new one using the <b>touch .gitignore</b> command on the <b>gitbash</b> cli otherwise, another CLI will not recognise this command</li>
            <li>add the names of <b>folders</b> you want to ignore.</li>
            <li>Rung <b>git add .</b> to stage all the new changes.</li>
            <li>run <b>git commit -m</b></li>
            <li>check the remote connection name, then run <b>git push origin main</b>, incase if the connection name is <b>origin</b> and branchname is <b>main</b></li>
            <li>run <b>git push origin main</b> OR <b>git push origin main --force</b></li>
            
</ol></li>
    </ol>

<h1>What git push -u Does</h1>
<ol type="1">
    <li>When you use <b>git push -u origin 'branch-name'</b> , you are telling Git to:
    <ol type="a">
        <li>Push the specified <b>local</b> branch to the <b>remote</b> repository (origin).</li>
        <li>Set the <b>upstream branch</b> for the <b>local</b> branch, which means that your local branch will be <b>linked</b> to the remote branch on the <i>specified remote repository (origin)</i>.</li>
    </ol></li>
    <li>Simplifies Future Pushes and Pulls:
        <ol type="a">
            <li>Once the upstream branch is set, you can simply use git push or git pull without specifying the remote and branch name. Git will remember the remote branch and automatically use it for future pushes and pulls.</li>
            <li><b>git push</b> and <b>git pull</b></li>
            <li>To track the <b>status</b> use <b>git status</b></li>
            <li>It helps keep track of changes and ensures that everyone is working on the correct branches, reducing the chance of errors in collaborative environments.</li>
            <li>To check which <b>upstream</b> is the <b>local branch</b> tracking: <br>
            <b>git branch -vv</b></li>

        </ol>
    </li>
</ol>

<h1>References</h1>
    <ol type="1">
        <li>Apna College Video Tut: <a href="https://www.youtube.com/watch?v=Ez8F0nW6S-w&list=PLuVUjM2teP9bnLNS8FV_e-1eiL1ZV8W2k&index=1&t=2436s">Link</a></li>
        <li><b>Changing name of default branch from gitHub.</b><br>
        <img src="/images/defaultNameChange.PNG" alt=""></li>
    </ol>
</body>
</html>