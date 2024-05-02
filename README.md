# devops_demo
This repo is created for demonstration of devops activities

#### 1. Download and Install Visual Studio Code
#### 2. Open the Workspace directory in VSC
#### 3. Modify the file content in Workspace
#### 4. Go to GitBash and check the status
    $ git status
    $ git add FileName
    $ git status
    $ git commit -m ""

#### 5. Generate Token Key from GitHub (Profile -> Settings -> Developer Settings -> PAT -> Tokens)
    $ git push origin master
        Git Hub UN and Token Key

#### 6. Goto GitHub and check the latest changes / verify the commits also

#### 7. How to resolve Conflicts
    # pull the code from remote repo
    $ git mergetool (Open the file in vimdiff)
    # edit the conflict file (4th editor) and save it
    # commit and push the file to remote repo

#### Directory Structure:

##### - Creating a Branch
		Ex: Master -> Dev
		    Dev -> Feature

        Formula:
            Src -> Dest
                $ git checkout Src
                $ git branch dest

##### - Committing to Branch
		Ex: commit to Dev

        Formula:
            - Identify the branch to commit
            - $ git checkout branch_name
            - $ git commit 

##### - Merging Branches
		Ex: Feature -> Dev
		    Post Release:
			- Release -> Master
			- Release -> Dev
  
        - Formula:
            -  Src -> Dest (Feature -> dev)
                $ git checkout dest_branch
                $ git merge src_branch

##### - Backup of Branches (Master/main)
		- Tagging
            Ex: 'main' has to take backup
                'feature' has to take backup

        - Formula:
          - $ git checkout branch_name
          - $ git tag tag_name

#### Diff Command:
	- To check the diff bet workspace file with Local repo (git diff)
	- To check the diff bet staging files with local repo (git diff --staged)
	- To check the diff bet current commit comparing with previous commit (git show commit_id)
	- To check the diff bet branches (git diff branch1 branch2)