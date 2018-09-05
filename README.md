# CST407SRSDOD
Data Oriented Design

Project Name(s):  

    - DOD

Purposes:  

    - Understand Data Oriented Design.  
    - Learn to use C++ concurrency library.  
    - Practice using the C++ random number generator and clocks.  

Specification:  

Create an contiguous array of bytes (std::byte or unsigned char) in 2 dimensions.  
Fill the array with random values in the range \[0, 256).  
Create N C++ threads or N C++ tasks to calculate the number of values greater than M where M is \[0, 256).  

The tests use:  
- Number of threads and/or number of tasks.  
- Thread global increment of total array vs thread local increment of total array.  
- Row and column order traversal of the data.  
- Maximum value threshold.  

Count the number of values that exceed the threshold.  

Measure the time it takes to complete and graph it as the dependent variable.  

Before coding, write your hypothesis for the results.  

You will create 2 graphs as follows:

1) Row/Column Major  

Independent variable:  
- Where N == \[1, 5000), create square array\[N]\[N] (Tip: Use a vector<byte> and divide into chunks.)  

Compare:  
- Row vs Column order traversal.  

Constants:  
- Single threaded.  
- Maximum value threshold == 127.  

---

2) Thread Local Storage

Independent variable:  
- Number of threads.  

Compare:  
- Thread global increment of total array vs thread local increment of total array.  
- Maximum value threshold == 10 and 200.  

Constants:  
- Row order traversal  
- Thread concurrency (not tasks)  
- Where N == 5000, create square array\[N]\[N] (Tip: Use a vector<byte> and divide into chunks.)  

###
