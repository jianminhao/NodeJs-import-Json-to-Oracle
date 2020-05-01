# NodeJs-Utils
Convert Json file into Oracle insert statement

Utilities I developed for managing JSON files and databases.

Import JSON to Oracle database insert SQL Statements.
Input: folder Name, which contains JSON files in second level subfolder. 
Output: insert SQL statement (Oracle Style). 
Calling method: ImportJSON2SQL -r rootPath -l Logpath 
rootPath: required, root folder for HTML. 
LogPath: optional, if not specified, will use rootpath.

This program is written in NodeJS javascript, it uses JSON to parse Json file.

Running this program will generate two files: insert_date.sql and processed.txt. Eachtime you run the program,
it will check the processed.txt to see whether a folder is processed or not. If it is processed, this program will skip processing it.

Sample JSON file:
{
  "ID": "S1797",
  "fullmetrics": [
    {
      "aID": "A14871",
      "panels": [
        {
          "panel": "1",
          "metrics": [
            {
              "a": "Pgroup",
              "b": "14871",
              "c": "2525.33",
              "d": "1917.79",
              "e": "0.00"
            }
          ]
        }
      ]
    }
       
  ]
}


