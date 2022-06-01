# This are my notes about git github :computer: to:cloud:



| Windows              | Unix                |
| -------------------- | ------------------- |
| cd                   | cd                  |
| dir                  | ls                  |
| mkdir                | mkdir               |
| del/rmdir            | rm -rf              |
| comes from the Shell | comes from the bash |

* dir/ls => lists the directories
* cd (directory name) => change directory
* cd .. => return to the directory above
* cls => clear screen
* tab => autocompletion
* mkdir => make directory
* (>) => directs the action into a directory
* flags => /S, /Q



## Internal objects of GIT

#### BLOB - TREES - COMMITS

1. Blobs contains metadata  of GIT
   * object type
   * string size
   * file size
   * stores the file's SHA1

2. Tree stores Blobs
   * stores the SHA1
   * file name
   * sets the structure of where the files are
3. Commit is the object the unifies the other 3
   * points to a tree (SHA1)
   * points to a parent (SHA1)
   * points to an author
   * points to a message
   * the SHA1 of the commit is the hash of all the information

## Codes

* git config --global user.email "email"
* git config --global user.name "name"

sets/defines email and user name. It is important to use the same github credencials once they will be stored as authors within the commits.



*  git init .

initializes a ghost subdirectory from an already existing repository.



* git add "name of the file" / git add . / git add *

starts the monitoring of the files. Change the file status to monotored.



* git status

verifies the status of the added file on master branch.



* git commit -m "message"

commit is the object of GIT that gives meaning to the alterations. Stores the indices actual content of a new commit along with a message of the user registered describing the changes (used after git add)

* git remote -v

shows the linked address



### Sequence of commands to add files 

* git init -b main
* git add .
* git commit -m "message"
* git remote add origin "github pathway"
* git push --set-upstream origin master



