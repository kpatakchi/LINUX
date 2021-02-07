
### File Transfer/Management:
For more information, check this link:
https://www.2daygeek.com/copy-files-folders-linux-cp-command/

##### Copy Files

`cp -R` or `cp -r`: Both are recursive copy, meaning that cp copies the contents of directories, and their sub-directories as well.

Ex:

Copy my dataset into p/project/kiste:
`scp -r ./patakchiyousefi1/00-DATASET/ patakchiyousefi1@juwels.fz-juelich.de:/p/project/kiste/patakchiyousefi1/`

#### Move Files

 The `mv` command doesn't have an `-R` flag, it moves folders recursively: 
 
`sudo mv fromPath/ toPath/`

Ex:

`mv /p/project/kiste/patakchiyousefi1/04-PROJECTS-SIMLINK ~`


### Mount Cluster in Local Using SSHFS:

Ex: Load p/project/kiste/patakchiyousefi1 in a sshfs folder:

`sshfs patakchiyousefi1@juwels.fz-juelich.de:/p/project/kiste/patakchiyousefi1/ ~/kiste_sshfs/`


