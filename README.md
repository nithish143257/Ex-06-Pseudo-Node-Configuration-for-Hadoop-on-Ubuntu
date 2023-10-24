# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

### Single-Node Configuration

1.	Create a dedicated user account for hadoop

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/ca29c68d-ec78-45aa-b0ac-eb00162c33eb)

2.	Install java1.8 in folder /usr/local                                                         

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/502fee64-f30b-4a59-91c7-d1475c6bf0f5)

3.	Install Hadoop

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/56ce94bb-ef68-4dd0-8fd4-2800e8e046c1)

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/a6279aa3-65e0-4fa5-9bcc-5717f00480df)

5.	Set hadoop environment variables: Include the following lines /etc/profile file

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/ef23d388-6cf3-441d-919e-43d847e2ae1c)

6.	Run the.bashrc & profile files from the $ prompt for updating the changes

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/bede731d-1511-491b-851a-debecaf6142c)

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/1636f8a7-f3ed-4ef2-a899-18aee6c6fc9c)


7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/5cc29292-af78-4134-a391-936126936b41)

b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/fe1d3117-ebe8-4e45-9a5b-6e0ce7dcc8c6)
 
Include the following lines in core-site.xml file between <configuration> and </configuration> tags

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/bcb631fc-443b-4f89-a6a5-dbe6b20c6af5)

c)	mapred-site.xml
 
![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/16683c44-3349-49fc-a3e0-2dcd2279be60)

Include the following lines in mapred-site.xml file
 
![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/0aba4901-920c-4e0b-8281-f3ce0edbfef6)

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/50b2db98-e09a-4ea9-ac66-25f21aad2bdc)

e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/93a4a5a7-bb9b-4e50-b825-14a2956ec309)

8.	Format the Hadoop File system implemented on top of the local file system using

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/629fc485-bdfd-426d-9c9e-1044538c97d9)

9.	Start Hadoop using

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/1e0dd3b2-33ea-4941-a2cc-df23641d382c)

Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/64bbdd38-2eb6-4921-8f96-967af69db990)

11.	Create a directory ‘/input’ in HDFS

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/b57b3b22-2a67-4346-a4c2-4e3aabdcd34f)

12.	Copy the input files into the distributed file system

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/d02e9532-39b5-46f0-a4a2-fe1ece4f0a52)

13.	Run some of the examples provided

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/ee7d811c-e2b2-405b-9b68-b46b2f000113)

14.	Examine the output files

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/cc8b73ba-f51b-4f8b-86d3-a2ddd53d840f)

Copy the output files from the distributed file system to the local file system and examine them:

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/c5f25553-0013-4b1b-8319-25af48e53389)

or

View the output files on the distributed file system

![image](https://github.com/nithish143257/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/113762839/989294b9-8bc5-4930-88c9-1221aa4c7677)

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
