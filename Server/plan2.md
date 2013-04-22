#Exeter Computing Club Server Plan

##Introduction
The ECC server is meant to be a place where ECC developers can host projects. These projects should be built for servers; the server is _not_ meant as a computer on which you can do remote computations. It will also serve as a portal between non-ECC members and ECC members.

##Setup
The server will be built on a LAMP (ArchLinux and Apache HTTPD 2.4) structure. It will include the following software:
 - gcc/g++
 - java (6 and 7)
 - python (2.7 and 3.3)
 - pip (2 and 3)
 - sqlite3
 - mysql
 - ruby (1.9 and 2.0)
 - rvm
 - perl
 - git
 - svn
 - ssh

##The end-user experience
The landing page of the ECC server will be a sort of club portal; it will include links to current projects and also contain a weblogesque channel containing club news. The only endpoint not handled by a club-member project will be the root (http://ecc.exeter.edu and http://ecc.exeter.edu/index.html). Each project will have a root directory; for instance, ecc.exeter.edu/project1/* would strictly be handled by project1's files and scripts.

If ECC grows large enough that this becomes practical, we may also launch an http endpoint for project management (database editing, read/write to project files).

##Project development
Currently (since ECC is such a small club), project development will happen over ssh. Each project will have a directory (e.g. project1), and the admins will register the project's endpoint (http://ecc.exeter.edu/project1/*). Until we come up with a better system, all files in the project directory will be run as executables if marked as executable in linux (e.g. chmod +x), served as plaintext files if not, and ignored (return 404 not found) if directories.

##Administration and privileges
The club adviser (currently Mr. Sea) will have root access on the server. Administrators (a position appointed by Mr. Sea) will have sudo access to the entire filesystem _except_ the sudoers file. SSH clients (club members) will have access to certain project directories; these permissions will be handled by the administrators. Any person may apply for SSH access relatively easily; accounts will be managed by the administrators. However, SSH clients will begin with _no_ priveleges, and will be granted access to project directories when they write proposals for contributions to projects.

The job of the administrator is basically to make things less of hassle for the club adviser:
 - To grant and remove SSH client permissions to project directories (they should be _very_ reserved about changing permissions; they should grant access only with a proposal and an application, and revoke it only when someone has broken pre-established rules).
 - Managing the landing site (index.html).
 - Updates to the server meta-software (installing patches to ArchLinux and Apache, installing the latest versions of interpreters and database clients while still maintaining backward compatability)
 - Notifying ECC club members when their projects are taking ugly amounts of computing power or space, and then acting to preserve service (e.g. by terminating processes or deleting files) if project developers do not fix their software in time.

The club adviser will be the only one with regular access to the server machine itself. 

###The http commit endpoint
If ECC grows large enough that this is practical, we may also write an http endpoint that allows non-SSH clients to host projects. They will register for developer accounts on ecc.exeter.edu (managed through a standard library password storage scheme) and then be allowed to, via http requests:
 - commit changes to the project directories to which they have access
 - execute daemons and cron jobs

This endpoint will monitor file size, and will fail to commit if it exceeds a reasonable amount (to be decided if and when this endpoint is actually launched).

##Version control
_Every project directory_ will be a git respository. Project members will have permission to commit their changes to the local git respository, and push the commits to the corresponding github repository (which will be made under the Exeter organisation) at will. The administrators will also run a cron job automatically committing and pushing all directories once per day.


