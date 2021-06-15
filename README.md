# Twitter-analysis
This is the intermediate part of a project which aim is to create a twitter bot which will perform the following tasks:
1) Download tweets of all main political parties in Poland and store them in the Postgres database. 
2) Transform the data to calculate various statistics (e.g. word frequency) for each political party.
3) Visualize the data in a dashboard form in real time. 

Initial data exploration and analysis part is placed in the analysis file.
The following components of the tool has been already completed:
1) Creation of AWS RDS database (Postgres SQL).
2) Creation of an ETL pipeline (listener file) which collects tweets, transforms them (cleans them and counts words) and loads to the RDS database.
3) Dashboard which queries SQL db and presents the data based on aggregation chosen by an user (dashboard file and png screen).

Remaining steps to finish the tool:
- Setting up AWS EC2 instance and deploying the listener script
- Refining the dashboard (adding data table option etc.) and deploying it to Heroku.
