# Components of Web Application:

### Login:
	
* Authentication
* Authorization

### Request Filter:
* Encode set
* Custom http header set
* log add
* redirect url
	
### Request & Session Listener:
* Request and Session Log add
* Session-wise variable set and unset
	
### Database & ORM:
* OneToOne Relationship
* OneToMany Relationship
* ManyToMany Relationship
* Cascade Delete & Update
* Batch Insert
* ORM level Caching

### Application Logging:
* Set log file location
* Log file splitter
* Set Log level

### Mail Sending:
* SMTP Configuration
* Mechanism for Testing Mail using dummy sender

### Caching:
* Web Resource caching(e.g. CSS, JS, Image, HTML, Font file cache)
* Cache Service to preload most used data from DB (e.g. memcache, radis)

### Jobs:
* Scheduled Job to do transfer data from one source to another or record status change
* Scheduled Job to backup Whole Database
* Scheduled Job send mail
* Async Job to process long requested task(e.g. parse a large xml submitted by http post, image thumbnail create)
* Async Job to Log some event (e.g. login success or failed log, db record change log)
* Async Job to send mail to user
	
### Searching Tools and Techniques:
* Database Indexing
* Caching tools. e.g. Memcache, radis
* NoSQL Storage. e.g. ElasticSearch, ApacheSolr
