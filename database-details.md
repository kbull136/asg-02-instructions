# Database Details

## overview

All data used on the website flows from a database that you need to create, populate with tables, and then populate with data.

The database consists of these following tables:

1. cities
2. continents
3. countries
4. imagedetails
5. imagerating (not used in this year's assignment)
6. languages
7. postimages (not used in this year's assignment)
8. posts.sql (not used in this year's assignment)
9. users.sql
10. userslogin.sql

This might sound like hard work...but it's not. 'cause there's a script for that.

## the database creation script

The script is available here in the assignment 2 repo. It's called [travel-3rd.sql](travel-3rd.sql).

## database creation and population on XAMPP

I've created a [walkthrough of the process](https://youtu.be/rkO443kfFuk) [4:11] to use the above script to create the database and populate the tables in XAMPP.

## database creation and population on Heroku

### ClearDB MySQL

Heroku itself does **not** natively use mySQL, so an add-on (ClearDB MySQL) is required. The process of setting it up isn't nearly as painful as I feared it was going to be.

Watch these screencasts in order:

1. [getting mysql onto your heroku box](https://youtu.be/n-25KMMZjkM) [8:04]
2. [getting the travel tables into ClearDB](https://youtu.be/AcIdqDZlYCk) [7:05]


### Google Cloud Platform (GCP) MySQL 

If, for whatever reason, don't want to use a credit card to use ClearDB, you can get things working with a GCP MySQL instance.

Watch these screencasts in order:

1. [applying Google Cloud Platform (GCP) credits](https://youtu.be/bs0VOP3KiM0) [6:35] 
2. [creating a GCP project](https://youtu.be/0OSHSaeetwA) [3:32] 
3. [overview of what we're trying to do with GCP](https://youtu.be/I3DbbhabyN0) [4:30] 
4. [creating a mySQL instance on GCP](https://youtu.be/EF--K_Kmovc) [8:52] 
5. [connecting to our GCP server via the mySQL client](https://youtu.be/H_5_1yQO_1U) [16:30] 
6. [setting up environment variables on Heroku for GCP](https://youtu.be/Ecw_6Tj-nXg) [7:55] 

### IMPORTANT, YO

You only want ONE ClearDB/GCP database for the Heroku site - not one for each group member. So have ONE member do the setup and then share the configuration information with the rest of the group.

_Because I think **everyone** should share this experience, guess what kind of thing you're all doing for tutorial 10?...._

## further setup (optional)

If you want to expend a bit of extra effort, you can configure your PHP site so that your PHP code "just works" whether it's running on XAMPP or on Heroku. It uses a lot of the same steps that were covered in [lecture 18](https://youtu.be/b8FT8KQfCdU).

Walkthrough: https://youtu.be/YNljMRhRkAA [37:40]
