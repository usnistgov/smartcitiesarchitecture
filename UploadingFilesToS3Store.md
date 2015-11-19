# Managing Files for NistPagesTemplate

## Installation of tools
For windows:

1. install [AWS Command Line Tool](http://docs.aws.amazon.com/cli/latest/userguide/installing.html)

1. install [Python](https://www.python.org/ftp/python/2.7.10/python-2.7.10.msi)

1. Add python path to environment path variable
a.	Python 2.7 will install to C:\Python, and pip.exe to C:\Python\Scripts. 
b.	Add these to the path using Control Panel: System: Advanced System Settings: Environment Variables: System Variables: Path  and edit that by appending ;C:\Python to the end 

1. Use the Python "pip" program to install additional tools:
    C:\Python27\Scripts\pip install beautifulsoup4
    C:\Python27\Scripts\pip install requests-ntlm
    C:\Python27\Scripts\pip install boto

1. Add a template for credentials in %USERPROFILE%\.aws
a.	Add a “.aws” sub-directory under C:\Users\USERNAME using command prompt “mkdir .aws” from >C:\Users\USERNAME 
b.	Use Notepad++ to create a file (with contents below, 5 lines, which serves as the template for credentials) and save as “credentials.”


Contents of %USERPROFILE%\.aws\credentials. file:

	[default]
	output = json
	region = us-west-2
	aws_access_key_id = 
	aws_secret_access_key = 

## Test your configuration
1. Open a command window in the NistPagesTemplate main directory
1. run the command:

	initializeCredentials.py

1. you will be asked for your NIST general realm login credentials
1. if successful it will print out "Access valid"
1. a successful login will enable access for up to an hour after which credentials would have to be reentered

## How to add a file
1. Open a command window in the NistPagesTemplate main directory
1. Place files to be uploaded in the files directory according to the file tree organization desired in S3 
1. Run yamlDocumentRecord.py to produce entry in documents file (use the relative path to the file to be uploaded in the files directory)


		Usage: yamlDocumentRecord.py filename title description category team
		<filename> is a filename to use
		<title> is title
		<description> is description
		<category> is one of "document" | "presentation" | "TEapproach" | "standard" | "video" | ""
		<team> is a team mnemonic string we will create and use


1. When presented with the yml code, if acceptable, answer Y and file will be copied to aws and the _data/documents.yml file will be appended with the record.
1. When done, commit and check in changed documents.yml file
 