# Background
HTML5 WebSQL databases are currently available in Safari (including Mobile Safari), and the HTML5 FileAPI is implemented in Phonegap.

Unfortunately the WebSQL API wasn't prescriptive in a number of areas; there is no canonical method of furnishing your HTML5 offline app with a pre-populated SQL database.

It took me quite a while to figure out how to get this to work reliably - so here's the solution.

# Requirements
This example web page will run inside phonegap, and probably any other HTML5 browser that supports SQL and File.

# What is it
A demonstration of how to pre-populate an HTML5 webSQL database using a textfile created by the sqlite .dump command. 

# Usage (phonegap)
Copy the index.html file into your phonegap app /www folder

Create your SQL seed file from a SQLite database using the command:

    sqlite .dump <database_name> > dump.sql
    
If using phonegap, copy the dump file into your www folder.
    
Edit the SQL_DUMP_FILE global variable.

Compile and run.
    
# License
BSD

