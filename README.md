# RfC_dumper
Parses and dumps given Wikipedia RfCs' content, author information etc. into a MySQL database

## Requires...
1. Requires python 2.X

2. Install MySQLdb 1.3.9

## How to run it.
1. git clone https://github.com/trusttri/RfC_dumper.git

2. `cd RfC_dumper`

3. Before running the script, create a new database called *wikum*. Dump "wikum.sql" (which is in /RfC_dumper/db) to it (`mysql -u root -p wikum < wikum.sql`). It's important that the name of database is *wikum*, since I fixed the name in grab_rfcs.py.

4. Run the script: `python grab_rfcs.py [name of json file] [password of DB]`. For example in my case it was `python grab_rfcs.py rfcs_amy.json Scott605`


## Tested on..
Tested on Windows 7 and 8, using Python 2.7 and MySQLdb 1.3.9
