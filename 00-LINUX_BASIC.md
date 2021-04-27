
### 1. File Transfer/Management:
For more information, check this link:
https://www.2daygeek.com/copy-files-folders-linux-cp-command/

##### 1.1. Copy Files

`cp -R` or `cp -r`: Both are recursive copy, meaning that cp copies the contents of directories, and their sub-directories as well.

Ex:

Copy my dataset into p/project/kiste:
`scp -r ./patakchiyousefi1/00-DATASET/ patakchiyousefi1@juwels.fz-juelich.de:/p/project/kiste/patakchiyousefi1/`

#### 1.2. Move Files

 The `mv` command doesn't have an `-R` flag, it moves folders recursively: 
 
`sudo mv fromPath/ toPath/`

Ex:

`mv /p/project/kiste/patakchiyousefi1/04-PROJECTS-SIMLINK ~`


#### 1.3. Create a Simlink

Specify the directory name as the first parameter and the symlink as the second parameter.

` ln -s source simlink`

Ex: Simlink projects (kiste project) in HDFML

` ln -s /p/project/kiste/ ~/PROJECT_SYMLINKS `


##### 1.4. Delete Files

Delete a single file:

`rm filename`




### 2. Mount Cluster in Local Using SSHFS:

Install 

`sudo apt-get install sshfs`

Ex: Load p/project/kiste/patakchiyousefi1 in a sshfs folder:

`sshfs patakchiyousefi1@juwels.fz-juelich.de:/p/project/kiste/patakchiyousefi1/ ~/kiste_sshfs/`


