# System Puzzle Weblog

# Problem
A system using Postgresql, RabbitMQ, nginx, Python, and docker.  RabbitMQ is ingesting weblog files and storing the results in Postgresql. nginx and flask are used as the frontend to display the percentage of GET requests in the logs were successful.  

The creator of this system is new to the technologies utilized and needs help troubleshooting it.  

Also added support for local / remote statistics of GET requests.  

For more information:  https://github.com/InsightDataScience/System-Puzzle-Weblog  


# List of uncovered problems
Problem: failure to bind due to conflicting port usage of nginx and ingestion services.  
Problem:  nginx isn't pointing to the same port as it's configuration says it is  
Problem:  db didn't initialize the schema.  
Problem:  unicode errors being thrown from ingestion.py  
Problem:  processing.py issues with basic_consume  
