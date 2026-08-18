#install jenkins repo from official doc 
#install java-21-openjdk , enable and start  jenkins service after installation , jenkins runs on port 8080

#/var/lib/jenkins/secrets/initialPassword - for initaila password
#/var/lib/jenkins/secrets/jobs - jobs 
#/var/lib/jenkins/workspace  - files created

#All jenkins plugin have .hpi(Hudson plugin) extension ---> plugin.jenkins.io

###JENKINS VARIABLE##
---------------------
#Pre-configured variables:

BRANCH_NAME
    For a multibranch project, this will be set to the name of the branch being built, for example in case you wish to deploy to production from master but not from feature branches; if corresponding to some kind of change request, the name is generally arbitrary (refer to CHANGE_ID and CHANGE_TARGET).
BRANCH_IS_PRIMARY
    For a multibranch project, if the SCM source reports that the branch being built is a primary branch, this will be set to "true"; else unset. Some SCM sources may report more than one branch as a primary branch while others may not supply this information. 
CHANGE_ID
    For a multibranch project corresponding to some kind of change request, this will be set to the change ID, such as a pull request number, if supported; else unset.

##refer the jenkins console for more..
------

##local variable : Declare the variable inside Build steps>> execute shell
##Global variables: Manage jenkins >> Systems >> environment variables

---------------------------------------------
#Build with paramanters: pick job>configure>general>"This project is parameterized"

--------------------------------------------
#SCM-Trigger
github integration with Jenkins

