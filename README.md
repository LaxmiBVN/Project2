# Project2
# Books Webservice


1. Database named 'cat' containing table named 'test' has been created in mysql on Amazon EC2.

2. Commands used:
    # create database test;
    # use database test;

3. Created table named 'cat' using:
    #CREATE TABLE cat ( work_id varchar(255) default null, obj_id varchar(255) default null, rev_no varchar(255) default null, time varchar(255) default null, info varchar(2000) default null);

4. Copied the cat-works.txt from host to EC2 using
    # scp -i key.pem /path/to/myfile.txt ec2-user@IPAddressOfEC2:

5. Loaded data from text file into database using:
    # LOAD DATA INFILE 'cat-works.txt' INTO TABLE cats;

6. Created a python file prjct2.py that contains the code to fetch data as per the problem statement.

7. Execution can be seen from any browser at the following address:

  http://54.244.41.255:5001/info/work_id
