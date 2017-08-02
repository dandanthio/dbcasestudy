# READ ME FIRST
You should just clone the source codes from our repo and skip to 'Prepare and create project in NetBeans Project'

# Getting and unpacking the .war file
* Get the latest one with other updated files here https://deliveringtechnology.atlassian.net/wiki/spaces/DT/pages/3539077/Updated+files
* Unpack files into C:\docker-image-files and overwriting the old ones.

# Unpack again
Unpack DBankWebTier.war into your desired folder (e.g. Git repo folder should be C:\Users\Graduate\Documents\GitHub\dbcasestudy\DBankWebTier )
You will find folders and files like
* META-INF folder
* WEB-INF folder 
* index.jsp file 

# Prepare for project
Reference: https://stackoverflow.com/questions/15226407/importing-existing-jsp-project-to-eclipse-or-net-beans
* Create new folder called 'web'
* Move WEB-INF and all files (NOT META-INF) into web folder

# Create project in NetBeans Project
* Open NetBeans and create project using existing sources under 'Java Web'
* Follow the wizard and tada!
- Location and project folder - C:\Users\Graduate\Documents\GitHub\dbcasestudy\DBankWebTier
- Server set it to Apache Tomcat
- Web pages folder - C:\Users\Graduate\Documents\GitHub\dbcasestudy\DBankWebTier\web
- WEB-INF folder - C:\Users\Graduate\Documents\GitHub\dbcasestudy\DBankWebTier\web\WEB-INF
- Libraries folder - C:\Users\Graduate\Documents\GitHub\dbcasestudy\DBankWebTier\web\WEB-INF\lib

# Test
* Press Run Project (F6) button and your browser should show the HTML from DBankWebTier\index.jsp
* If you did not set up your mySQL server (via Docker or even locally), you should see 'DB NOT CONNECTED' message.
* Find the How-to set up mySQL server container to test your app's database connection.