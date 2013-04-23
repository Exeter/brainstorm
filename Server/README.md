#Exeter Computing Club Server

 - [Server Setup](https://github.com/Exeter/brainstorm/blob/master/Server/setup.md)
 - [Administration Guide](https://github.com/Exeter/brainstorm/blob/master/Server/administration.md)

####Metasoftware

 - [ecc-index](https://github.com/Exeter/ecc-index)
 - [exeter_server](https://github.com/Exeter/exeter_server)

##Mission
The Exeter Computing Club server is a student-run server with the purpose of serving a platform for PEA students and ECC developers to host web projects relevant to the PEA community. Our server will also used as a platform for other educational ECC projects.

#Production plan
This is the plan for the ECC server once it is put into production.
##Administration
The server will be located in Mr. Sea's office. The server will not be physically accessed under normal circumstances.

The club adviser, Mr. Sea will have full root access on the server. A team of administrators will have limited sudo privilleges.

###Administrators
Administrators will be given the responsibility of maintaining the server, e.g.:
- checking logs for suspicious behavior
- monitoring network traffic if need be
- creating accounts for
- making sure server deployments are running smoothly

Administrators will also be responsible for the development processes and procedures for server management. Server meta-software will be designed and engineered by the Administration team, or by appointment or assignment of the Administration team.

The job of Administrator is a selective job. Administrators will be appointed by co-heads, and will be chosen on the basis of trust, sanity, responsibility, and ability. But mostly trust. Administrators will also have to be approved by Mr. Sea.

The job of Administrator is a serious job. We will probably have you sign something or do a pinkie promise.

__(TODO: Define Administrator terms, conditions, and misuse)__

##Usage
###Student Projects

####Project hosting
Students will be able to store and provide their project of relevance to the PEA community for use on our server.
Projects will be reviewed via a web-based application process. Approved projects will be able to be deployed via some API we'll have to design. This method does not involve giving users shell accounts.

The application will probably look something along the lines of:
 - What is your project?
 - How is it relevant to the PEA community?
	
####Shell accounts
Students of the PEA community and CS club will be able to apply for an SSH account via written electronic application. This application include basic informational questions such as:
 - What is your project?
 - How is it relevant to the PEA community?
 - Why do you you need a shell account?
 - What will you do on the server?

__(TODO: Better define "misuse")__
Misuse of resources and trolling will NOT be tolerated. Misuse of resources is defined as the storage of inappropriate materials such as large meaningless texts or the use of space or computing power to perform things that are not specified in the application, such as arbitrary speed testing. Trolling is defined as any deliberate and intentional attempt to disrupt the usability of the server for its users and administrators, e.g. Denial of Service attacks, SQL injections, cracking SSH accounts.

The server will be setup to be as secure as possible, but trust is still of utmost importance. We'll have a one-strike policy, and if we can't trust you, you're out.

Users will be limited in terms of server resources, eg. memory, disk space, CPU usage (?) etc. Users exceeding or approaching these limits will get automatically notified via email, and, under extreme conditions, automatically suspended. Troublesome projects/ users will be taken down under administrator review if needed.
