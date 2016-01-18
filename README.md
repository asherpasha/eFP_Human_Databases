# eFP Human Databases

The databases in this repository are MySQL dumps of eFP Human data. To download this data, please install Git LFS system from: https://git-lfs.github.com/ . Then clone this Github repository to fetch the data. Decompress the data using xz (or parallel xz), and check the integrity of the data. On Unix/Linux operating systems it can done as follows after installing Git LFS (tested on Git version 2.1.4, Git LFS version 1.1.0 on Debian 8.2):

#### Cloning Git LFS repository

```sh
$git clone https://github.com/asherpasha/eFP_Human_Databases.git
$cd eFP_Human_Databases
$pxz -T 4 -d human_body_map_2.sql.xz
$pxz -T 4 -d human_developmental.sql.xz
$md5sum human_body_map_2.sql
$md5sum human_developmental.sql
```

#### Checking integrity of databases
The md5sum of the database on the server are:<br />
5dc756c6c5da1ddd7e22d8902a49668e  human_body_map_2.sql <br />
e91658ba77ff8110672b5086124b0f09 human_developmental.sql

#### Other Options
If you have trouble downloading the databases from github, you can download the databases directly from the BAR: <br />
http://bar.utoronto.ca/efp_human_databases/

Thank you.
