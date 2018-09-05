# CST276SRSDOD
Data Oriented Design

Project Name(s):  

    - DOD

Purposes:  

    - Learn to use C++ concurrency library.  
    - Understand Data Oriented Design.  

Specification:  

Create an 2 dimensional array of 479001600 total unsigned ints.  
Fill the array with random values \[0, 256).  
Divide the array into N chunks, where N is \[1, 33).  
Create N C++ threads or tasks to calculate the number of values greater than M where M is \[0, 256].  

For each test case collect data for the time it takes to complete and graph it. 

The independent variables are:  
- Number of threads/tasks.  
- Direct increment of total array vs thread local increment of total array.  
- Row vs Column order traversal of the data.  
- Maximum value threshold, choose 100 data points.  

Count the number of values that exceed the threshold.  

###
