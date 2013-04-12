#CS Club Server Plan

##Mission
Our student-run server will be used as a space for students and CS club to host projects relevant to the PEA community. Our server will also be used as a space for other CS club undertakings.

##Administration
The server will reside in Mr. Sea's office, and under ordinary circumstances will never be physically touched. Administration will take place remotely via SSH.

Only Mr. Sea will have root access. In addition to the co-heads, there will also be one or two other members on an Administration team that will have sudo privilleges. 

__(TODO: what extent of sudo privilleges? We need flexibility, but we should also follow the principle of least privillege)__

###Administrators
Administrators will be given the responsibility of maintaining the server, eg:
- making sure nothing fishy is going on, by:
	- checking logs
	- monitoring network traffic
- making sure server deployments are running smoothly

Administrators will also be responsible for developing processes and procedures for server management. Server meta-software will be designed and engineered by the Administration team.


The job of Administrator is a selective job. Administrators will be appointed by co-heads, and will be chosen on the basis of trust, sanity, responsibility, and ability. But mostly trust. Administrators will also have to be approved by Mr. Sea.

The job of Administrator is a serious job. We will probably have you sign something or do a pinkie promise.

__(TODO: Think of ways to make the administration process as democratic and transparent as possible, but also as streamlined and secure as possible)__

##Backups
Back up once a week? once a day?

##Usage
###Student Projects
__Sean wrote down Anthony's idea of a non-shell based project hosting, but Sean thinks until we get big, we can simplify things by having just application-based shell acounts for hosting a few projects__

####Anythony's idea
Students will be able to host their project of relevance to the PEA community on our server.
Projects will be reviewed via a web-based application process. Approved projects will be able to be deployed via some API we'll have to design. This method does not involve giving users shell accounts.

The application will probably look something along the lines of:
	- What is your project?
	- How is it relevant to the PEA community?
####Shell accounts
Students of the PEA community and CS club will be able to apply for a shell account via written application. This application will probably look something along the lines of:
	- What is your project?
	- How is it relevent to the PEA community?
	- Why do you you need a shell account?
	- What will you do on the server?

Fishyness will not be tolerated. The server will be setup to be as secure as possible, but trust is still of utmost important. We'll have a one-strike policy, and if we can't trust you, you're out.
__TODO: define fishiness in better, more specific terms__

Shell accounts will expire in 30 days(?) so we'll have some automatic renewal process.

##Setup
Operating System: Arch Linux
__(TODO: Document specs and hardware)__


