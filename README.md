# Udacity-FSWDND-Project-5
This is the repository for my submissionf or the Udacity Full Stack Web Developer Nanodegree project 5.  This only contains the README file for the project.

SSH IP address: 52.26.83.98:2200
Public URL: http://ec2-52-26-83-98.us-west-2.compute.amazonaws.com/

Software installed (various prerequesites and dependencies not shown):
	apache2
	libapache2-mod-wsgi
	postgresql
	git
	python
	python-pip
		flask 
		sqlalchemy 
		oauth2client 
		httplib2 
		flask_restless
	fail2ban

Configuration changes made:
	Added a user called 'grader', gave it a password, added that user to the SUDO group, and copied root's SSH key to grader.
	Installed the above-mentioned software along with their dependencies.
	Changed the default SSH port to 2200.
	Set up UFW to block everything except ports 80, 123, and 2200.
	Installed fail2ban, and changed maxretry to 6.  Ban time remains at 600 seconds.
	Configured Apache to serve the Catalog app, and changed the settings on my Google Developer Console to allow the Amazon virtual machine's URL.
	Set up SUDO to execute without prompting for a password.