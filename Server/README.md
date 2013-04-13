#Exeter Computing Club Server Plan

##Mission
Our student-run, instructor-supervised server with a .exeter.edu domain name will be used as a space and medium for students and CS club to host projects relevant to the PEA community. Our server will also be used as a space for other CS club undertakings.

##Administration
The server will be located in Mr. Sea's office, and under ordinary circumstances will never be physically touched. Administration will take place remotely via SSH. However, it will be accessed if conditions warrant.

Only Mr. Sea will have root access. In addition to the co-heads, there will also be one or two other members on an Administration team that will have sudo privileges. 

__(TODO: what extent of sudo privilleges? We need flexibility, but we should also follow the principle of least privillege)__

###Administrators
Administrators will be given the responsibility of maintaining the server, e.g.:
- making sure no trolling is going on, by doing the following regularly:
	- checking logs
	- monitoring network traffic
- making sure server deployments are running smoothly

Administrators will also be responsible for the development processes and procedures for server management. Server meta-software will be designed and engineered by the Administration team, or by appointment or assignment of the Administration team.

The job of Administrator is a selective job. Administrators will be appointed by co-heads, and will be chosen on the basis of trust, sanity, responsibility, and ability. But mostly trust. Administrators will also have to be approved by Mr. Sea.

The job of Administrator is a serious job. We will probably have you sign something or do a pinkie promise.

__(TODO: Think of ways to make the administration process as democratic and transparent as possible, but also as streamlined and secure as possible)__

###Backups
Back up weekly or daily?
__Problems with storage.__

##Usage
###Student Projects
__Sean wrote down Anthony's idea of a non-shell based project hosting, but Sean thinks until we get big, we can simplify things by having just application-based shell accounts for hosting projects__

####Project hosting
Students will be able to store and provide their project of relevance to the PEA community for use on our server.
Projects will be reviewed via a web-based application process. Approved projects will be able to be deployed via some API we'll have to design. This method does not involve giving users shell accounts.

The application will probably look something along the lines of:
 - What is your project?
 - How is it relevant to the PEA community?
	
####Shell accounts
Students of the PEA community and CS club will be able to apply for an SSH account via written electronic application. This application include basic informational questions such as:
 - What is your project?
 - How is it relevent to the PEA community?
 - Why do you you need a shell account?
 - What will you do on the server?

Misuse of resources and trolling will NOT be tolerated. Misuse of resources is defined as the storage of inappropriate materials such as large meaningless texts or the use of space or computing power to perform things that are not specified in the application, such as arbitrary speed testing. Trolling is defined as any deliberate and intentional attempt to disrupt the usability of the server for its users and administrators, e.g. Denial of Service attacks, SQL injections, cracking SSH accounts.
The server will be setup to be as secure as possible, but trust is still of utmost importance. We'll have a one-strike policy, and if we can't trust you, you're out.

Users will be limited in terms of server resources, eg. memory, disk space, CPU usage (?) etc. Users exceeding or approaching these limits will get automatically notified via email, and, under extreme conditions, automatically suspended. Troublesome projects/ users will be taken down under administrator review if needed.

In general, the server should not be used for computing, but only for storage or service.

Shell accounts will expire in 30 days(?) so we'll have some automatic renewal process.
__Disagreed.__

##Setup
Operating System: Arch Linux
__(TODO: Document specs and hardware)__


