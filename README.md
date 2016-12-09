# Project2
# Books Webservice


1. Database named 'cat' containing table named 'test' has been created in mysql on Amazon EC2.

2. Commands used:
    # create database test;
    # use test;

3. Created table named 'cat' using:
    #CREATE TABLE cat ( work_id varchar(255) default null,object_id  varchar(255) default null, rev_no varchar(255) default null, timestamp varchar(255) default null, details text default null);

4. Copied the cat-works.txt from host to EC2 using
    # scp -i key.pem /path/to/myfile.txt ec2-user@IPAddressOfEC2:

5. Loaded data from text file into database using:
    # LOAD DATA INFILE 'cat-works.txt' INTO TABLE cat;

6. Created a python file prjct2.py that contains the code to fetch data as per the problem statement.

7. Execution can be seen from any browser at the following address:

  http://ec2-54-191-163-142.us-west-2.compute.amazonaws.com:5001/search/word </br>
  http://ec2-54-191-163-142.us-west-2.compute.amazonaws.com:5001/work/id
  
8. Sample output:
   http://ec2-54-191-163-142.us-west-2.compute.amazonaws.com:5001/work/OL15058106W </br>
 {"Timestamp": "2010-04-28T07:54:43.266997", "Author Name": "Dandi Daley Mackall", "details": {"created": {"type": "/type/datetime", "value": "2010-04-17T05:45:53.003152"}, "title": "The great meow mystery", "covers": [1285725], "last_modified": {"type": "/type/datetime", "value": "2010-04-28T07:54:43.266997"}, "latest_revision": 2, "key": "/works/OL15058106W", "authors": [{"type": {"key": "/type/author_role"}, "author": {"key": "/authors/OL32072A"}}], "type": {"key": "/type/work"}, "subjects": ["Fiction", "Christian life in fiction", "Christian life", "Cats in fiction", "Lost-and-found possessions in fiction", "Cats", "Lost-and-found possessions", "Mystery and detective stories"], "revision": 2}}
  


  
