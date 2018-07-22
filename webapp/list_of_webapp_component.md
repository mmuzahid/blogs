# Components of Web Application:

### Login:
	
* Authentication: Check User Credential at DataSource
* Authorization: Check Role, Permission to Access Resources

### Request Filter:
* Set Request Character Encoding
* Set Custom HTTP headers
* Add Log to Log File
* Redirect to other URL
	
### Request & Session Listener:
* Add Log to Log file to trace Request and Session
* Initialize some Session-wise Long Process. e.g. Fetch Session Info From DB 
* Session-wise variable set and unset

### Database & ORM:
* OneToOne, OneToMany, ManyToMany Relationship
* Cascade Delete & Update
* Batch Insert
* ORM Level Caching

### Application Logging:
* Set Log File Location. e.g. Appender at Log4j
* Set Format of Log Entry
* Set Log File Splitter Logic
* Set Log level. e.g. INFO, DEBUG, ERROR

### Mail Sending:
* SMTP Configuration: host, port, authenticator
* Setup a Test Environment without Sending to Real Receiver

### Caching:
* Web Resource Caching(e.g. CSS, JS, Image, HTML, Font file cache)
* Cache Service to preload most used data from DB (e.g. MemCache, Radis)

### Jobs:
* Scheduled Job to transfer data from one source to another or record status change
* Scheduled Job to backup Whole Database
* Scheduled Job to send mail
* Async Job to process long task(e.g. parse a large xml submitted by http post, image thumbnail create)
* Async Job to Log some event (e.g. login success or failed log, db record change log)
* Async Job to send mail to user
	
### Searching Tools and Techniques:
* Database Indexing
* Caching tools. e.g. Memcache, radis
* NoSQL Storage. e.g. ElasticSearch, ApacheSolr, MongoDB

### Web Server Setup:
* Set Certificate File Location in Web/Application Server. e.g. httpd-ssl.conf in Apache2 , server.xml in Tomcat
* Virtual Host Setup. e.g. Allow Server to serve for different hostname
* Load Balancer Setup. e.g. worker configuration in apache2 and tomcat
* URL Rewrite Logic. e.g. Rewrite to a default context, Redirect to a URL based on requested URL hostname or path 
* Enable Admin/Manager User. e.g. tomcat-users.xml in Tomcat
