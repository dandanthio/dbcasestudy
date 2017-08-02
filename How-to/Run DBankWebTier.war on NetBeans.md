# READ ME FIRST
You should just clone the source codes from our repo and skip to 'Prepare and create project in NetBeans Project'

# Getting and unpacking the .war file
Get the latest one with other updated files here
https://deliveringtechnology.atlassian.net/wiki/spaces/DT/pages/3539077/Updated+files

# Unpack
Unpack files into C:\docker-image-files and overwriting the old ones.

# Unpack again
Unpack DBankWebTier.war into your desired folder (if you are not using our GitHub repo)
You will find folders
* META-INF
* WEB-INF
and files like
* index.jsp

# Prepare and create project in NetBeans Project
Reference: https://stackoverflow.com/questions/15226407/importing-existing-jsp-project-to-eclipse-or-net-beans
* Create new folder called 'web'
* Move WEB-INF and all files (NOT META-INF) into web folder
* Open NetBeans and create project using existing sources under 'Java Web'
* Follow the wizard and tada!

# Test
Press Run button and your browser should show the HTML from DBankWebTier\index.jsp