Project Name: NFS_Award_Tracing

Description:
ProjectTrace is a data processing and analysis tool that traces the lifecycle and progress of projects funded by federal agencies. It retrieves project data from various sources, performs topic modeling on project abstracts and titles, creates a database of project information, and generates insights and statistics to assess the impact of the projects on society.

Directories: 

- dashboard -  For customized visual interface. Directory needed by to be inserted into the XAMPP > htdocs folder upon installation

- External_Scraping - Directory intended to be used to grow DB to 10 GB (was not implemented) contained advanced coding to scrape data.
	> topicmodeling.py: Python module containing functions for topic modeling
	> links.py - would gather links for sraping based on the topic modeling keywords
	> data.py - Python module containing functions for data processing (based on links)
	> toSQL.py - Would transfer the html data from data.py into a mySQL db.

-NSF - Core directory with databases and the backbone of the php interface
	>  webscrapper.py - Original python webscraper file used to gather the data from nfs.gov in 	between others.

-index.php - contains script to load the rigth interface files from dashboard when accessing the localhost server.

-NSF_Tracing_Report.pdf -  Report of findings

Usage:
1. Install the XAMPP Software developed by Apache

2. Access the deafult xampp folder > htdocs > copy all of the files in this directory (replace existing ones)

3. Run XAMPP Control Panel and then run both the Apache server and MySQL Modules  

4. From any browser, access localhost. Redirection to the interface will occurr automatically

5. Explore the awards and manage the database from the web interface


