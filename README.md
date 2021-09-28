# HIVE Project
# Associate Management System - AMS 

# Project Description:

The main aim of this project is to manage the database of an educational institute that provides courses in various domains. It consists of associate details like how many associates were attended for a demo, joined, enrolled for the courses like Bigdata, IoT, machine learning, artificial intelligence, etc. Whenever the administrator needs information about the associates, they should be able to fetch the required data.


# Technologies :

1)Cloudera5 <br>
2)Hadoop <br>
3)Hue <br>
4)MySQL <br>
5)Sqoop <br>
6)Github <br>
7)Microsoft Excel <br>
8)Microsoft Powerpoint <br>


# Features :

1.Availability of multiple courses, Discounts on each course. <br>
2.Availability of demo sessions on weekdays as well as weekends. <br>
3.Rescheduling of demo session if missed. <br>
4.Multiple payment modes. <br>
5.Installments availability on any types of payment mode. <br>
6.Availability of both Online and Offline mode of training. <br>
7.Updation can be performed on master table. <br>

# Tables :

1) Master and Payment Tables in MySQL <br>
2) Enquiry Table <br>
3) Demo Schedule - Weekday_Demo and Weekend_Demo tables <br>
4) Demo_Attended and Demo_Missed Tables <br>
5) Course Enroll Table <br>
6) Not_Joined Table <br> 
7) Payment Table <br>

# Enquiry Table
Enquiry Table is an orc table that is created by loading the data of master table in it. It consists of the entire information of the assosiates who are enrolled for the institute like Name, age, Email, Mobile_no , Course, Fee, Discount, Demo_Date, status_final 

# Demo Schedule Tables
We have two tables to hold the demo scheduled associates details depending on their demo modes namely Weekday and Weekend Demo tables. We created this tables by extracting the data from our enquiry table. The associates who have scheduled their demo on weekday are stored in Weekday demo table and the associates who are scheduled their demos are stored in weekend demo table.

# Demo Attended Table
It is taken from enquiry table who has done their demo with added attributes like demoday (WD,WE),day,time

# Demo Missed Table
Data for this table taken from enquiry table whose status is DND and adding attributes like reschedule_datetime

# Course Enroll Table
This table holds the details of the associates who are enrolled for the courses and we created two tables that holds associate details who opt for weekdays and weekend modes

# Not Joined Table
This table holds the details of the associates who are not enrolled to course after finishing their demo. This data is extracted from master table having status as NJ

# Payment Table
This table is created from table4.txt data that consists of the payment details of the associates who are enrolled for the courses consisting the payment details of the associates like total fee, fee paid, mode (any installment), mode of payment, number of installment, end date for payment

# Contributions :

1. Eswar Naidu - Data Analytics <br>
2. Neha - Database Management <br>
3. Suleman - Data Collection preprocessing <br>
4. Subodh Kumar - Quality Assurance <br>
5. Gaurav Mishra - Development <br>
